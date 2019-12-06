# Sagas

A Saga function will look like this

```javascript
//action will take the whole action, which is triggered in the action.js file
export function* getTeamByIdSaga(action) {
  // Select username from store
  const username = action.value;
  const requestURL = `https://api.github.com/users/${username}/repos?type=all&sort=updated`;

  console.log(requestURL);
  try {
    // Call our request helper (see 'utils/request')
    const repos = yield call(request, requestURL);
    console.log(repos);
    yield put(teamIdChangeSUCCESS(repos, false));
  } catch (err) {
    console.log(err);
    yield put(teamIdChangeError(err, false));
  }
}
```
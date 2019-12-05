# Actions

A action will possibly look like these:

```javascript
import {
  DEFAULT_ACTION, INCREMENT,
} from './constants';

export function incrementAction(value) {
  return {
    type: INCREMENT,
    value,
  };
}
```
 In the reducer file like this:
 ```javascript
import { fromJS } from 'immutable';
import {
  DEFAULT_ACTION, INCREMENT,
} from './constants';

const initialState = fromJS({});

function storeTestReducer(state = initialState, action) {
  switch (action.type) {
    case DEFAULT_ACTION:
      return state;
    case INCREMENT:
      // console.log(action, state);
      return state.set('value', fromJS(action.value));
    default:
      return state;
  }
}
 ```

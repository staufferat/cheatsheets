#React-Router

#Imports
```
npm i --save react-router-dom
npm i --save react-router-redux
```

##Navigation
```html
<NavBar>
  <HeaderLink to="/">
    <FormattedMessage {...messages.home} />
  </HeaderLink>
  <HeaderLink to="/test">
    Test
  </HeaderLink>
</NavBar>
```
In the Navigation we use "Link to" and push a String which is linked to the React Component

##Link to the Components

```html
<Switch>
    <Route exact path="/" component={HomePage} />
    <Route exact path="/test" component={StoreTest} />
    <Route path="/features" component={FeaturePage} />
    <Route path="" component={NotFoundPage} />
</Switch>
```

##Create Redux Store with history

```javascript
import createHistory from 'history/createBrowserHistory';

const initialState = {};
const history = createHistory();
const store = configureStore(initialState, history);
const MOUNT_NODE = document.getElementById('app');
```

##Import the Router in the app.js
```javascript
<ConnectedRouter history={history}>
    <App />
</ConnectedRouter>
```


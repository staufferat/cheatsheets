# Store

## Boilerplate

If you use boilerplate, the Store is already created and configured in the store.js.



It's recommended to use an "initialstate", this looks like this:

```javascript
const initialState = fromJS({});
```
In the Reducer function set initialState as state.

```javascript
function loginReducer(state = initialState, action) {  
    switch (action.type) {    
        case DEFAULT_ACTION:      
            return state;    
        case USER_CHANGE:      
            return state.set('value', fromJS(action.user));    
        default:      
            return state;  
    }
}
```
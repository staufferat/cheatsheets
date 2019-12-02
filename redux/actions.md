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

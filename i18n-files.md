#i18n messages

##Messages
A messages.js file looks like following:
```javascript
/*
 * ShiftMessageForm Messages
 *
 * This contains all the text for the UserLoginForm component.
 */
import { defineMessages } from 'react-intl';

export default defineMessages({
  header: {
    id: 'app.components.ShiftMessageForm.header',
    defaultMessage: 'Idoc hochladen und upserten',
  },
  idoc: {
    id: 'app.components.ShiftMessageForm.idoc',
    defaultMessage: 'idoc XML',
  },
  submitButton: {
    id: 'app.components.ShiftMessageForm.submitButton',
    defaultMessage: 'Speichern',
  },
});

```

# sms-global-js
A node js library for the SMS global http-api.

## Installation
```
npm install --save sms-global-js
```

## Usage
```
const SMSGlobal = require('sms-global-js');

const sms = new SMSGlobal();

sms.authenticate('username', 'password');
sms.setFromName('Example');
sms.setRecipient('+645555555555');
sms.setMessageBody('This is a test sms from JS!');

sms.send().then((res) => {
  // do something cool, because you just sent a sms.
}).catch((err) => {
  // something's not right here.
});
```

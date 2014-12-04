# A Node Client for Narad
## Installation
```bash
$ npm install narad
```
## How to use
```javascript

var Narad = require('narad');

var narad = new Narad({
  appId: 'YOUR-NARAD-APP-ID',
  key: 'YOUR-NARAD-APP-ID',
  secret: 'YOUR-NARAD-SECRET-KEY',
  domain: 'api.nrtt.in', //defaults to localhost
  port: 4567 // defaults to 4567
});

var channel = 'lobby',
    event = 'message',
    data = {
      from: 'Hitesh',
      content: 'Hello World'
    };

narad.trigger(channel, event, data, function (err, req, res) {
  //do something (callback is optional)
});

```

## License
This code is free to user under the terms of the MIT license.
# MessageSMS

Resources: 
[Nexmo](https://www.nexmo.com/)\n
[GitHub](https://github.com/Nexmo/nexmo-node)

## Installation

```bash
npm install nexmo --save
```

## Constructor

```js
var Nexmo = require('nexmo');

var nexmo = new Nexmo({
    apiKey: API_KEY,
    apiSecret: API_SECRET,   
  });
```

* `apiKey` - API Key from Nexmo
* `apiSecret` - API SECRET from Nexmo


## Send text message
```js
nexmo.message.sendSms(
    'URVIRTUALNUMBER', number, text, { type: 'unicode' },
    (err, responseData) => {
      if(err) {
        console.log(err);
      } else {
            //Do domething with the response
        }
      }
    }
  );
});
```

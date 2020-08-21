# qiao-is-online-browser
is online on browser by load img

## install
```
npm install qiao-is-online-browser
```

## api
### isOnline
```javascript
'use strict';

var q = require('qiao-is-online-browser');

var test = async function(){
    try{
        var isOnline = await q.isOnline();
        console.log(isOnline);

        // var isOnlineByYourImg = await q.isOnline(your img src);
        // console.log(isOnlineByYourImg);
    }catch(e){
        console.log(e);
    }
};

test();
```

### offlineToOnline
```javascript
'use strict';

var q = require('qiao-is-online-browser');

// callback
// time, interval time, default is 3*1000ms
q.offlineToOnline(function(){
    console.log('offline-to-online');
}, 3 * 1000);
```

## version
### 0.0.1.20200821
1. init project
2. offline to online
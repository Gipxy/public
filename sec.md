* ReDOS: regular expression DOS

```javascript
let c = function (n) {
  let d1 = new Date();
  let s = '!';
  for (let i = 0; i < n; i++) {
    s = 'a' + s;
  }
  r = s.match('^(([a-z])+.)+[A-Z]([a-z])+$');
  d2 = new Date();
  console.log('time:', n, d2 - d1);
};

c(45);
```
Output: n=45, time=60s => hang for 60 seconds

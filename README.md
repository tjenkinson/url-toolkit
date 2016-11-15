[![Build Status](https://travis-ci.org/tjenkinson/url-toolkit.svg?branch=master)](https://travis-ci.org/tjenkinson/url-toolkit)

# URL Toolkit
Lightweight library to build an absolute URL from a base URL and a relative URL. Initially part of [HLS.JS](https://github.com/dailymotion/hls.js).

## Example
```javascript
var URLToolkit = require('url-toolkit');
var url = URLToolkit.buildAbsoluteURL('https://a.com/b/cd/e.m3u8?test=1#something', '../z.ts?abc=1#test');
console.log(url); // 'https://a.com/b/z.ts?abc=1#test'
```
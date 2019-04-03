# Mock.js - async version

仅修改Mock.mock方法使支持Promise异步数据替换

使用方式如下:

```javascript
Mock.mock(/foo\/bar/, function(){
    return new Promise(resolve=>{
        setTimeout(resolve, 3000, {data:"模拟的数据"});
    })
})
```


[![Build Status](https://travis-ci.org/nuysoft/Mock.svg?branch=refactoring)](https://travis-ci.org/nuysoft/Mock)

[原版主页](http://mockjs.com/)

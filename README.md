# Mock.js - async version

仅修改Mock.mock方法使支持Promise异步数据替换

安装:
```bash
yarn add -D mockjs-async 
npm install --save mockjs-async
```

使用:
```javascript
import Mock from "mockjs-async"

Mock.mock(/foo\/bar/, function(){
    return new Promise(resolve=>{
        setTimeout(resolve, 3000, {data:"模拟的数据"});
    })
})
```


[![Build Status](https://travis-ci.org/nuysoft/Mock.svg?branch=refactoring)](https://travis-ci.org/nuysoft/Mock)

mockjs完整功能，请查阅 [原版主页](http://mockjs.com/)

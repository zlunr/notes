#1. webpack的起源？
#2. webpack发展历程？
#3. webpack特性？

#4. 如何利用webpack？
* 打包index.js
```
const path = require('path');   //引入路径插件

module.exports = {
  entry: './src/index.js',  //需要打包的文件路径
  output: { //输出
    path: path.resolve(__dirname, 'dist'),  //输出路径（__dirname 为根目录，dist为需要创建的文件夹名称）
    filename: 'bundle.js'   //输出打包后文件的名称
  }
};
```
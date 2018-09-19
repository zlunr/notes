# npm 使用
## 初始配置
```
//设置初始用户邮箱
$ npm set init.author.email "wombat@npmjs.com"
//设置初始用户名
$ npm set init.author.name "ag_dubs"
//设置初始用户协议
$ npm set init.license "MIT"
```
## npm下载安装包
`npm install <project name>`
> dependencies 生产环境
> devDependencies 开发环境
> global 全局安装
> ```
> $ npm install <package_name> --save
>$ npm install <package_name> --save-dev
>$ npm install <package_name> -g
>```
## 常用命令
`$ npm update`  更新模块
`$ npm uninstall <package_name>`    卸载模块
`$ npm uninstall --save lodash`     同时从package.json文件中移除

## 配置npm源
当我们使用默认配置从npm官网下载模块时，由于网络的因素，会导致我们的下载速度特别慢。所以，我们可以配置一些国内的镜像来加快我们的下载速度。推荐使用[淘宝的npm镜像](淘宝 NPM 镜像), 具体使用方式如下:

+ 临时使用, 安装包的时候通过--registry参数即可

  `$ npm install express --registry https://registry.npm.taobao.org`
+ 全局使用

  `$ npm config set registry https://registry.npm.taobao.org`
  // 配置后可通过下面方式来验证是否成功
 ` npm config get registry`
  // 或
  `npm info express`
+ 使用cnpm使用

  // 安装cnpm
  `npm install -g cnpm --registry=https://registry.npm.taobao.org`

  // 使用cnpm安装包
  `cnpm install express`

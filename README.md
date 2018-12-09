# learnvue

> A Mpvue project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

### 使用mpvue模板
vue init mpvue/mpvue-quickstart my-project
cd my-project
npm install

### 下载腾讯云
https://console.qcloud.com/lav2 下载node.js 的zip包
把server文件copy到项目中
```
cd server 
npm install
```

#### 本地搭建小程序开发环境
https://cloud.tencent.com/developer/ask/25171 
<br>
进入文件 project.config.json 
设置腾讯云地址 `"qcloudRoot": "server/"`,
进入文件server/config.js 
<br>
设置腾讯云的id及其配置
<br>
// 腾讯云相关配置可以查看云 API 秘钥控制台：https://console.cloud.tencent.com/capi
``` js
serverHost: 'localhost',
tunnelServerUrl: '',
tunnelSignatureKey: '27fb7d1c161b7ca52d73cce0f1d833f9f5b5ec89',
qcloudAppId: '1256686025',
qcloudSecretId: 'AKID76tUt6zxZzFJAojYcar33rSs6A3lJfrr',
qcloudSecretKey: 'ylQqAIiKp8IJ8mIix0udAVfdVbd4PZXK',
wxMessageToken: 'weixinmsgtoken',
networkTimeout: 30000,
```

解决问题： 更新代码之后不再重启项目
在server目录下安装 nodemon 
```
npm install nodemon --save
```
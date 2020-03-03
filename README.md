# jweixin-npm
封装最新微信jweixin-1.6.0.js文件的NPM

## Usage

#### Install

```sh
$ npm install --save jweixin-npm
```

## Example

```js
import wx from 'jweixin-npm'

wx.config({
  debug: true, // 开启调试模式,调用的所有api的返回值会在客户端alert出来，若要查看传入的参数，可以在pc端打开，参数信息会通过log打出，仅在pc端时才会打印。
  appId: '', // 必填，公众号的唯一标识
  timestamp: 1560503719000, // 必填，生成签名的时间戳
  nonceStr: '', // 必填，生成签名的随机串
  signature: '', // 必填，签名
  jsApiList: ['openLocation', 'chooseImage', 'previewImage', 'uploadImage', 'downloadImage', 'chooseWXPay'] // 必填，需要使用的JS接口列表
})

```

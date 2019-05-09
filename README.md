> Wechat App(微信小程序, .wxapkg)解包及相关文件(.wxss, .json, .wxs, .wxml)还原工具

## 1. 说明
> - [x] 修复 “ReferenceError: $gwx is not defined” 和 extract wxss 等问题
> - [x] 支持分包
> - [x] 支持一键解包
> - [x] 支持一键安装各种依赖

### 2. wxapkg 包的获取

Android 手机最近使用过的微信小程序所对应的 wxapkg 包文件都存储在特定文件夹下，可通过以下命令查看：

    adb pull /data/data/com.tencent.mm/MicroMsg/{User}/appbrand/pkg ./

其中`{User}` 为当前用户的用户名，类似于 `2bc**************b65`。

## 3. 用法


- 解包某个小程序

```bash
node wuWxapkg.js 小程序包路径(.wxapkg格式)
```

** 举例

```bash
node wuWxapkg.js testpkg\_-751579163_42.wxapkg
```


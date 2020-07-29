# DCUniMPPresentCustomAnimation

### 简介

iOS 端 uni小程序SDK 打开小程序时采用的是present ViewController 的方式，默认从页面下方打开，本工程通过自定义专场动画的方式实现从页面右侧打开，类似 push 的效果；

### 使用教程

clone 或 下载工程源码，然后直接拖到工程中即可；

### 实现原理

通过 Hook 系统的 `presentViewController:animated:completion:`和 `dismissViewControllerAnimated:completion:` 方法为小程序对应的`DCUniMPViewController`设置 delegate，并提供自定义专场动画，当然您也可以根据需求自行修改动画方式；


想了解更多请看 UniMPSDK 官方文档：[自定义专场动画](https://nativesupport.dcloud.net.cn/UniMPDocs/Sample/ios?id=%e8%87%aa%e5%ae%9a%e4%b9%89%e5%8a%a8%e7%94%bb)

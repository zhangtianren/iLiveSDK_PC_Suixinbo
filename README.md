# iLiveSDK
iLiveSDK整合了音视频SDK(AVSDK)、即时通讯SDK(IMSDK)两大模块，致力于提供一套完整的音视频即时通讯解决方案。iLiveSDK 提供了账号登录，音视频互动，屏幕共享，收发消息等功能。旨在无限可能地降低用户接入成本，全方位考虑用户接入体验，并提供接入服务技术支持。

## iLiveSDK导入
[iLiveSDK导入参考](https://github.com/zhaoyang21cn/iLiveSDK_PC_Demos/blob/master/doc/iLiveSDK_README.md)

## SDK最近更新说明
### V1.9.0.2(2018-07-12)
* 修改SDK内部默认通道为云上环境(**老用户需要在初始化SDK后将通道设置为IMSDK通道，否则无法与旧版本互通;云上环境privateMapKey为必填字段**);
* 增加设置通道接口setChannelMode;
* 增加自定义数据透传接口fillCustomData;
* 修改进房参数RoomOption的authBuffer字段为privateMapKey;

[更多版本更新信息](https://github.com/zhaoyang21cn/iLiveSDK_PC_Demos/blob/master/doc/iLiveSDK_ChangeList.md)

## DEMO
[随心播编译及运行](https://github.com/zhaoyang21cn/iLiveSDK_PC_Suixinbo/tree/master/suixinbo)<br/>
[随心播运行包下载](http://dldir1.qq.com/hudongzhibo/git/iLiveSDK_PC_Suixinbo/suixinbo_run.zip)

## API文档
[API文档](https://zhaoyang21cn.github.io/iLiveSDK_Help/pc_help/annotated.html)

## 错误码
[错误码表](https://github.com/zhaoyang21cn/ILiveSDK_Android_Demos/blob/master/doc/ILiveSDK/error.md)

## 相关知识
[角色配置](https://www.qcloud.com/document/product/268/10620)<br/>
[如何录制混流视频](https://www.qcloud.com/document/product/268/10526)<br/>
[大咖模式](https://github.com/zhaoyang21cn/iLiveSDK_PC_Suixinbo/blob/master/doc/bigstar.md)<br/>
[跨房连麦](https://github.com/zhaoyang21cn/iLiveSDK_PC_Suixinbo/blob/master/doc/linkRoom.md)<br/>
[视频渲染](https://github.com/zhaoyang21cn/iLiveSDK_PC_Suixinbo/blob/master/doc/videoRender.md)

## 关键路径LOG
[关键路径LOG 请遇到问题先自行对比](https://www.qcloud.com/document/product/268/7752)

## 常见问题
[常见问题](https://github.com/zhaoyang21cn/iLiveSDK_PC_Demos/blob/master/doc/iLiveSDK_QA.md)

## QAVSDK下载
iLiveSDK内部集成了腾讯云的IMSDK和QAVSDK。使用iLiveSDK的用户不需要额外集成IMSDK或QAVSDK，就可以直接使用其所有功能。

对于仍在集成QAVSDK的老用户，也可以在这里获取QAVSDK的最新版本:

[QAVSDK_1.9.8.2](http://dldir1.qq.com/hudongzhibo/git/iLiveSDK_PC_Suixinbo/AVSDK/QAVOPENSDK_1.9.8.2_Windows_Publish.zip)

## 技术交流群
QQ群: 594923937

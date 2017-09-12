# iLiveSDK常见问题

## win32控制台程序收不到回调
iLiveSDK的回调依赖windows消息循环来抛回主线程,所以,程序中必须要有消息循环,且主线程不能阻塞，才能收到sdk的回调,即在main函数的末尾加上消息循环，如下,

```c++
MSG msg;
while( GetMessage(&msg, NULL, 0, 0) )
{
	TranslateMessage(&msg);
	DispatchMessage(&msg);
}
```

## 收到打开摄像头事件，却收不到视频数据回调
建议用户在后台SPEAR上将“实时通信”模式改为“互动直播”模式，“实时通信”模式长时间未维护，可能有不稳定因素;

## 关于视频渲染
iLiveSDK负责将视频数据抛给用户层，用户需要自己做渲染，可以参考随心播的渲染代码;<br/>
注意: sdk在第一次打开摄像头时，会去腾讯云后台拉取用户在Spear上配置的分辨率参数;所以，在拉取到配置前(约1~2秒)，sdk会以默认分辨率（320*240）回调给用户;
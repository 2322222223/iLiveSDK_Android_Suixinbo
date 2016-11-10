# ILiveSDK
ILiveSDK 提供了账号登录，音视频互动，文本互动等基础功能，顺利的话一天之内即可集成音视频能力。

支持以下场景     
>* [视频聊天类](./ILVLiveManager.md)
     类似now直播,映客 一人直播,多人观看,发文本消息,赞,送礼物。[具体参考](./ILVLiveManager.md)
>* [视频聊天类](./ILVCallManager.md) 
     类似微信视频通话功能呢,支持多人同时上麦(最多4路)。[具体参考](./ILVCallManager.md)

##ILiveSDK导入
ILiveSDK在Android Studio上开发。
导入只需要在gradle里增加一行（后面是版本号）,查看[版本更新说明](./release note.md)

compile 'com.tencent.ilivesdk:ilivesdk:0.3.5'



            
##DEMO
有三个示例  <br />
1视频聊天 ：双人通话场景的简单示例，类微信视频聊天。    
2基础直播 ：互动直播基础演示基础功能 登录进房间 加入房间 发消息 自定义消息等     
3新随心播 ：基于ILiveSDK接口重构的随心播        
##API文档
[API文档](https://zhaoyang21cn.github.io/ilivesdk_help/android_help/)

##已知问题

由于目前只支持armeabi架构，如果工程(或依赖库)中有多架构，需要在build.gradle中添加以下配置
<pre>
android{
    defaultConfig{
        ndk{
            abiFilter 'armeabi'
        }
    }
}
</pre>

如果您还在使用eclipse进行Android的开发，请参考这里[eclipse集成方案](./eclipse_readme.md)。    
Android Studio在google支持度，编译便利性等多方面远超eclipse。我们强烈建议还在使用eclipse的用户尽快升级。




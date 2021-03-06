# Android下音频对讲演示程序
# 必读说明

# 简介
#### 本软件根据《道德经》为核心思想而设计，实现了两个设备之间通过网络进行全双工实时音频对讲。为了增强对讲质量，还做了声学回音消除、噪音抑制、语音活动检测、自动增益控制、自适应抖动缓冲、等处理。

# 准备
#### 准备两台手机，要求安装了安卓2.3及以上的系统，其中一台手机作为客户端可以连接到另一台作为服务端的手机（可以用Ping工具测试，建议两台手机在同一WIFI下），且两台手机都安装相同版本的本软件。

# 开始
#### 在一台手机上直接点击创建服务端，再在另一台手机上将IP地址改为服务端手机的IP地址，并点击连接服务端，即可开始音频对讲，在任意端点击中断，即可中断音频对讲。
#### 设置按钮提供了各项功能的参数设置，绝大部分情况下都不需要修改，当然你也根据需要自行修改。
#### 特别注意：如果把两台手机放在同一房间里测试，很有可能会出现啸叫、声音不完整、等问题，这是因为现在手机的麦克风都很灵敏了，一点小小的声音都会被录进去，导致软件无法正确识别回音，所以建议放在不同的房间里测试。

# 其他
####     本软件采用了Speex的1.2rc2版本、SpeexDsp的1.2rc3版本、WebRtc为基础，并加入了本人自己设计的音频输入输出数据帧同步方法、自适应设置WebRtcAecm的回音延迟时间、自适应抖动缓冲器。声学回音可以消除到99%以上，且收敛时间很短，网络流量最大仅7KB/s。
#### 讨论QQ群：511046632    欢迎大家参与测试和讨论！
#### 本人QQ号：280604597    赤勇玄心行天道
#### 源代码下载地址：https://github.com/cyz7758520/Android_audio_talkback_demo_program

# 感谢
#### 感谢 WELEN、善书 对WebRTC的指点！
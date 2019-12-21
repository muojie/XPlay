[toc]

# 课程介绍
课程包含了对流媒体（拉流）的播放，演示了播放rtmp的香港卫视，支持rtsp摄像头和http网络视频的播放，支持访问本地的视频文件，并精确显示和控制播放进度：
1. 讲解如何编译Android平台的ffmpeg库，使其支持neon技术和硬解码，并测试性能
2. 使用opengles的NDK shader高效播放yuv视频，不耗费cpu性能更优（GPU）
3. 代码支持硬解码（省电不耗cpu）和多线程解码（高性能每秒解码240帧1080p）
4. 支持网络流媒体（rtmp，rtsp，http）可直接拉流播放电视并支持rtsp摄像头访问
5. 课程将设计模式应用到实践 - 观察者，构建者，门面，代理，适配器，单件模式

# 课程收益
1. 课程由浅入深，原理讲解+代码实操演示，并提供全部课程源码
2. 讲解如何编译Android平台的ffmpeg库，使其支持neon和硬解码，并测试性能
3. 使用opengles的NDK shader高效播放yuv视频，不耗费cpu性能更优




# Seek
- IDemux seek 关键帧问题，多线程暂停
- IDecode 解码缓冲，多线程暂停
- IAudioPlay 音频缓冲，多线程暂停
- IPlayer 控制 Seek

# 资源

## RTMP 在线测试地址（2019.04更新）
香港卫视,rtmp://live.hkstv.hk.lxdns.com/live/hks（已停用）  
这个rtmp url不是一直可用(2018年11月更新)，如不可用，可以访问以下两个url：

1. rtmp://live.hkstv.hk.lxdns.com/live/hks1

2. rtmp://live.hkstv.hk.lxdns.com/live/hks2


香港财经,rtmp://202.69.69.180:443/webcast/bshdlive-pc（推荐，信号好不卡顿）

韩国GoodTV,rtmp://mobliestream.c3tv.com:554/live/goodtv.sdp

韩国朝鲜日报,rtmp://live.chosun.gscdn.com/live/tvchosun1.stream

美国1,rtmp://ns8.indexforce.com/home/mystream

美国2,rtmp://media3.scctv.net/live/scctv_800

美国中文电视,rtmp://media3.sinovision.net:1935/live/livestream

湖南卫视,rtmp://58.200.131.2:1935/livetv/hunantv

原文链接：https://blog.csdn.net/zhichaosong/article/details/89053009

## RTSP协议直播源

大熊兔（VOD）：rtsp://184.72.239.149/vod/mp4://BigBuckBunny_175k.mov

国外电视台：rtsp://rtsp-v3-spbtv.msk.spbtv.com/spbtv_v3_1/214_110.sdp (2018年11月更新，暂不可用)，如果需要测试rtsp链接，可以用大牛直播SDK的 SmartPublisherDemo.exe 内置RTSP服务功能，生成个内网可用的rtsp url.

## HTTP协议直播源

香港卫视：http://live.hkstv.hk.lxdns.com/live/hks/playlist.m3u8

## 参考
https://github.com/CoderJackyHuang/MDArtileFiles/blob/master/%E7%9B%B4%E6%92%AD/%E7%9B%B4%E6%92%AD%E6%B5%8B%E8%AF%95%E5%9C%B0%E5%9D%80.md  
https://www.jianshu.com/p/20f9e9bb89aa  

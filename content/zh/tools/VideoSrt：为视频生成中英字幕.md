---
title: VideoSrt：为视频生成中英字幕
date: '2019-10-31T19:23:12+08:00'
tags:
  - 字幕
---
# VideoSrt：为视频生成中英字幕

本文发现自 @[小众软件](https://www.appinn.com/videosrt-for-windows/)，VideoSrt 是一款 Windows 下的开源工具，利用公共云服务接口，能够实现快速、批量的识别视频语音，并为视频自动创建中、英文字幕文件。

![VideoSrt](https://tva3.sinaimg.cn/large/6f8a2832gy1ga43g2846eg20ls0c8gu0.gif)

以下三个服务目前都有一定的免费额度，如果是个人普通需求的话，基本可以做到零付费，VideoSrt 基于阿里云 OSS 对象存储、阿里云录音文件识别以及百度翻译的接口 （by：VIGGO）

本身仅为开源软件，如需正常使用需要在相应平台申请 key 并填入软件中方可正常使用。

- [阿里云 OSS 对象存储](https://www.aliyun.com/product/oss)
- [阿里云录音文件识别](https://ai.aliyun.com/nls/filetrans)（试用版每日 2 小时时长）
- [百度翻译](http://api.fanyi.baidu.com/api/trans/product/index)（每月 200 万字免费）等服务



## 项目地址

https://github.com/wxbool/video-srt-windows
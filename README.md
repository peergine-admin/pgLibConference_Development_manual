```
一、系统概述

非常感谢您使用穿透科技的产品，我们将为您提供最好的服务。 

本手册可能包含技术上不准确的地方或排版错误。本手册的内容将做定期的 更新，恕不另行通知；更新的内容将会在本手册的新版本中加入。我们随时会改 进或更新本手册中描述的产品或程序。
```

* ### **1.1 系统介绍 **

AnyChat for Web SDK 是一套即时通讯开发平台（SDK），包含了音视频处理 模块、P2P 网络模块、音视频录制、文件传输、数据通信以及常见业务流程封装 等模块，是 AnyChat Platform Core SDK 的重要组成部分，专为 Web 浏览器设计， 即可以作为 PC 上的即时通讯，也可以作为视频会议、网络教育、文件传输、即 时抓拍等网络互动平台。AnyChat for Web SDK 支持所有主流浏览器，如 IE、 Google Chrome、Firefox 火狐浏览器等。整个平台由广州佰锐网络科技有限公司 独立研发，具有自主知识产权。 AnyChat SDK 分为客户端 SDK 和服务器 SDK 两大部分，其中客户端 SDK 用于实现语音、视频的交互以及其它客户端相关的功能，而服务器 SDK 主要实 现业务层逻辑控制，以及与第三方平台的互联等。AnyChat for Web SDK 属于客 户端 SDK，需要配合 Windows（或 Linux）的服务器程序才能正常工作。AnyChat for Web SDK 提供 JavaScript 编程接口。

## **1.2 系统特性**

AnyChat for Web SDK 采用增强的 H.264 视频编码算法和 AAC 语音编码 算法，具有高画质、语音清晰、流畅的特点，支持 P2P 技术进行网络传输，服务 器采用完成端口模型的重叠 IO，具有极高的并发处理能力。 AnyChat 服务器支持“SDK Filter Plus”和“AnyChat Server SDK”两种可扩 展编程接口，可方便实现与其它系统进行集成，增强 AnyChat 的可扩展性。上层 应用也可利用服务器 SDK 来实现更复杂的业务逻辑处理。可参考“AnyChat for Windows SDK”包中服务器开发相关文档。 第 6 页 共 65 页 AnyChat for Web SDK 开发手册 佰锐科技 版权所有 AnyChat 支持跨平台的应用，服务器支持 Windows、Linux、Unix 等所有主 流服务器操作系统，客户端目前支持 Windows、桌面 Linux、嵌入式 Linux、Web 浏览器、Android 平台、iOS 平台等。

### 1.2.1 视频技术

视频制式： PAL-B

分辨率： 176×144 —1920×1080（可调节）

帧 率： 5~30 FPS（可调节）

视频编码器：H.264

视频流码率：10kbps ~ 1000kbps（VBR）

支持硬件编码、解码（可定制，需提供对应平台的接口）

### 1.2.2 音频技术

采样率： 16000 Hz、22050Hz、44100Hz、48000Hz（可设置）

量化值： 16 bit

声 道： Mono、Stereo

音频编码器：AAC 音频流码率：6kbps ~ 128kbps

音效处理：回音抑制（AES）、噪音抑制（NS）、自动增益控制（AGC）、静音检测（VAD）

### 1.2.3 P2P技术

传输方式：UDP、TCP

支持的 NAT 类型：

Cone NAPT   Cone NAPT

Cone NAPT   Symmetric NAT

支持 UPNP 协议

## 1.3 关于佰锐科技

广州佰锐网络科技有限公司（GuangZhou BaiRui Network Technology Co., Ltd.）始创于 2005 年，是国内领先的网络语音视频技术研究与系统开发的高新 技术企业。十年来我们一直专注于音视频核心技术、基础数据通信能力研究，为 客户提供专业的音视频通信能力解决方案，打造了一款拥有独立知识产权、世界 一流的跨平台音视频解决方案产品“AnyChat”，该产品已成功应用于移动互联网、 物联网、在线教育、远程医疗、视频客服以及智能家居等业务领域，某些应用领 域占据整个行业 90%以上的市场份额。 成立十年以来，佰锐科技一直以“追求企业价值与客户价值共同成长”的 经营理念，已为数千家客户提供了优质的服务，凭借资深的研发团队和良好的口 碑，在激烈的竞争中脱颖而出，成为首屈一指的音视频能力解决方案提供商。 更多信息请参考佰锐科技官网：[http://www.bairuitech.com](http://www.bairuitech.com)

## 1.4 技术支持

在您使用 AnyChat SDK 的过程中，遇到任何困难，请与我们联系，我们将热 忱为您提供帮助。 您可以通过如下方式与我们取得联系：

1. 在线论坛：[http://bbs.anychat.cn](http://bbs.anychat.cn)

2. 公司官网：[http://www.bairuitech.com](http://www.bairuitech.com)

3. AnyChat产品网站：[http://www.anychat.cn](http://www.anychat.cn)

4. 电子邮件：service@bairuitech.com

5. 24 小时客服电话：+86 （020） 85276986、38109065、38103410

## 1.5 版权申明

“AnyChat for Web SDK”是由广州佰锐网络科技有限公司开发，拥有自主知识产权（软著登字第 066348 号）的系统平台， 广州佰锐网络科技有限公司拥有与本产品所用技术相关的知识产权。这些知 识产权包括但不限于一项或多项发明 专利或者正在进行申请的专利 （2006101239829、2006101241176）。 本产品发行所依照的许可协议限制其使用、复制分发和反编译。未经广州佰 锐网络科技有限公司事先书面授权，不得以任何形式或借助任何手段复制本产品 的任何部分。 随本 SDK 一同发布的 Demo 演示程序源代码版权归广州佰锐网络科技有限 公司所有。 AnyChat 是广州佰锐网络科技有限公司的商标。 第三方组件：AnyChat使用了开源的第三方组件，包括：FFmpeg（LGPL 2.1）、 libvpx（BSD）、libspeex（BSD）、WebRTC（BSD）。其中FFmpeg的版权所有者信 息、源代码以及其它信息均可在其官方网站：[http://www.ffmpeg.org找到。](http://www.ffmpeg.org找到。)


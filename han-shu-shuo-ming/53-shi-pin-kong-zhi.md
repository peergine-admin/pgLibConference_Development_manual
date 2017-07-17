## 5.3 视频控制

#### VideoStart: 初始化视频设置

`/**`

` *  描述：初始化视频设置`

` *  成员：iFlag[in] 参考1）静态成员定义：`

` *  阻塞方式：非阻塞，立即返回`

` *   返回值： true 操作成功，false 操作失败`

` */`

`public boolean VideoStart(int iFlag)`



#### VideoStop: 停止播放和采集视频

`/**`

` *  描述：停止播放和采集视频`

` *  阻塞方式：非阻塞，立即返回`

` */`

`public void VideoStop()`



#### VideoOpen: 打开某一成员的视频

`/**`

` *  描述：打开某一成员的视频`

` *  阻塞方式：非阻塞，立即返回`

` *   返回值： true 操作成功，false 操作失败`

` *   sPeer:成员节点名`

` *   iW: 窗口宽度`

` *   iH: 窗口高度`

` */`

#### VideoOpenL: 以不同流打开某一成员的视频（请求端有效）

`/**`

` *  描述：以不同流打开某一成员的视频（请求端有效）`

` *  阻塞方式：非阻塞，立即返回`

` *   返回值： true 操作成功，false 操作失败`

` *   sPeer:成员节点名`

` *   iW: 窗口宽度`

` *   iH: 窗口高度`

` */`

#### VideoReject: 拒绝打开某一成员的视频

`/**`

` *  描述：打开某一成员的视频`

` *  阻塞方式：非阻塞，立即返回`

` *   返回值： true 操作成功，false 操作失败`

` *   sPeer:成员节点名`

`*/`

`public SurfaceView VideoReject(String sPeer)`



#### VideoClose: 关闭某一成员视频

`/**`

` *  描述：关闭某一成员视频`

` *  阻塞方式：非阻塞，立即返回`

` */`

`public void VideoClose(String sPeer)`



#### VideoGetView: 获取已打开成员视频的View

` /**`

` *  描述：获取已打开成员视频的View`

` *  阻塞方式：非阻塞，立即返回`

` */`

`public SurfaceView VideoGetView(String sPeer)`



#### VideoControl: 控制成员的视频流

`/**`

` *  描述：控制成员的视频流`

` *  阻塞方式：非阻塞，立即返回`

` */`

`public boolean VideoControl(String sPeer, boolean bEnable)`



#### VideoSource: 摄像头切换

`/**`

` *  描述：摄像头切换`

` *  阻塞方式：非阻塞，立即返回`

` *  iCameraNo：摄像头编号`

` */`

`public boolean VideoControl(String sPeer, boolean bEnable)`






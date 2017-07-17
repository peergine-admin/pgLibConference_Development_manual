## 5.1 初始化及资源释放

### Initialize: 对象初始化函数：

`/**`

` *  描述：P2P会议对象初始化函数`

` *  阻塞方式：非阻塞，立即返回。`

` *  sName：[IN] 会议名称`

` *  sChair：[IN] 主席端设备ID`

` *  sUser：[IN] 登录用户名，自身的设备ID`

` *  sPass：[IN] 登录密码`

` *  sSvrAddr：[IN] 登录服务器地址和端口，格式：x.x.x.x:x`

` *  sRelayAddr：[IN] 转发服务器地址和端口，格式：x.x.x.x:x。`

` *                 如果传入空字符串，则使用登录服务器的IP地址加上443端口构成转发服务器地址。`

`*  sVideoParam：[IN] 视频参数，格式为：(Code){3}(Mode){2}(Rate){40}(LCode){3}(LMode){2} `

` *                 (LRate){40}(CameraNo){0}(Portrait){1}(BitRate){400}`

` *                 Code: 视频压缩编码类型：1为MJPEG、2为VP8、3为H264。`

` *                 Mode: 视频图像的分辨率（尺寸），有效数值如下：`

` *                        0: 80x60, 1: 160x120, 2: 320x240, 3: 640x480,`

` *                        4: 800x600, 5: 1024x768, 6: 176x144, 7: 352x288,`

` *                        8: 704x576, 9: 854x480, 10: 1280x720, 11: 1920x1080`

` *                 FrmRate: 视频的帧间间隔（毫秒）。例如40毫秒的帧率为：1000/40 = 25 fps`

` *                 LCode: 不同流视频压缩编码类型：1为MJPEG、2为VP8、3为H264。`

` *                 LMode: 不同流视频图像的分辨率（尺寸），有效数值如下：`

` *                        0: 80x60, 1: 160x120, 2: 320x240, 3: 640x480,`

` *                        4: 800x600, 5: 1024x768, 6: 176x144, 7: 352x288,`

` *                        8: 704x576, 9: 854x480, 10: 1280x720, 11: 1920x1080`

` *                 LFrmRate: 不同流视频的帧间间隔（毫秒）。例如40毫秒的帧率为：1000/40 = 25 fps`

`*                 InputExternal: 使能视频的外部采集`

`*                 OutputExternal: 使能视频的外部输出。输出解码后的视频帧，比如格式为RGB24`

`*                 OutputExtCmp: 使能视频的外部采集。输出未解码的视频帧，比如H264`

` *                 CameraNo: 摄像头编号，CameraInfo.facing的值。`

` *                 Portrait: 采集图像的方向。0为横屏，1为竖屏。`

`*                 Rotate: 采集图像的角度。`

` *                 BitRate: 视频压缩后的码率。单位为 Kbps`

` *`

` *  oCtx： Android程序的上下文对象`

` *  返回值：true 成功， false 失败`

` */`

`public boolean Initialize(String sName,String sChair, String sUser, String sPass, String sSvrAddr, String sRelayAddr, String sVideoParam, Context oCtx)`



### Initialize: 对象初始化函数：

`/**`

` *  描述：P2P会议对象初始化函数`

` *  阻塞方式：非阻塞，立即返回。`

`*  sUser：[IN] 登录用户名，自身的设备ID`

` *  sPass：[IN] 登录密码`

` *  sSvrAddr：[IN] 登录服务器地址和端口，格式：x.x.x.x:x`

` *  sRelayAddr：[IN] 转发服务器地址和端口，格式：x.x.x.x:x。`

` *                 如果传入空字符串，则使用登录服务器的IP地址加上443端口构成转发服务器地址。`

`*  sVideoParam：[IN] 视频参数，格式为：(Code){3}(Mode){2}(Rate){40}(LCode){3}(LMode){2} `

` *                 (LRate){40}(CameraNo){0}(Portrait){1}(BitRate){400}`

` *                 Code: 视频压缩编码类型：1为MJPEG、2为VP8、3为H264。`

` *                 Mode: 视频图像的分辨率（尺寸），有效数值如下：`

` *                        0: 80x60, 1: 160x120, 2: 320x240, 3: 640x480,`

` *                        4: 800x600, 5: 1024x768, 6: 176x144, 7: 352x288,`

` *                        8: 704x576, 9: 854x480, 10: 1280x720, 11: 1920x1080`

` *                 FrmRate: 视频的帧间间隔（毫秒）。例如40毫秒的帧率为：1000/40 = 25 fps`

` *                 LCode: 不同流视频压缩编码类型：1为MJPEG、2为VP8、3为H264。`

` *                 LMode: 不同流视频图像的分辨率（尺寸），有效数值如下：`

` *                        0: 80x60, 1: 160x120, 2: 320x240, 3: 640x480,`

` *                        4: 800x600, 5: 1024x768, 6: 176x144, 7: 352x288,`

` *                        8: 704x576, 9: 854x480, 10: 1280x720, 11: 1920x1080`

` *                 LFrmRate: 不同流视频的帧间间隔（毫秒）。例如40毫秒的帧率为：1000/40 = 25 fps`

`*                 VideoInExternal: 使能视频的外部采集`

` *                 CameraNo: 摄像头编号，CameraInfo.facing的值。`

` *                 Portrait: 采集图像的方向。0为横屏，1为竖屏。`

`*                 Rotate: 采集图像的角度。`

` *                 BitRate: 视频压缩后的码率。单位为 Kbps`

` *`

` *  oCtx： Android程序的上下文对象`

` *  返回值：true 成功， false 失败`

` * 与上面初始化函数的区别：上面的初始化函数在初始化登陆之后，同时初始化了会议。`

` */`

`public boolean Initialize(String sUser, String sPass, String sSvrAddr, String sRelayAddr, String sVideoParam, Context oCtx)`

``

#### Clean: 对象清理函数

`/**`

` *  描述：P2P会议对象清理函数`

` *  阻塞方式：非阻塞，立即返回。`

` */`

`public void Clean()`





#### WndCreate: 播放窗口创建函数

`/**`

` *  描述：创建播放窗口对象`

` *  阻塞方式：阻塞`

` *  iX：[IN] 窗口水平位置`

` *  iY：[IN] 窗口垂直位置`

` *  iW：[IN] 窗口宽度`

` *  iH：[IN] 窗口高度`

` *  返回值：SurfaceView对象，可加入到程序主View中`

` */`

`public SurfaceView WndCreate(int iX, int iY, int iW, int iH)`



#### WndDestroy: 播放窗口销毁函数

`/**`

` *  描述：销毁播放窗口对象`

` *  阻塞方式：阻塞`

` *  返回值：true 成功  false 失败`

` */`

`public void WndDestroy()`




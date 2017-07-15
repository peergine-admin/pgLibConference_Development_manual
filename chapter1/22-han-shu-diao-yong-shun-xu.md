| 调用顺序 | 方法 | 功能 | 说明 |
| :--- | :--- | :--- | :--- |
| A |  |  | 初始化 |
|  | new pgLibConference\(\); | 创建P2P会议对象 |  |
|  | new pgLibConference.OnEventListener\(\) | 创建事件回调接口对象 |  |
|  | SetEventListener\(\) | 设置事件回调接口对象 |  |
|  | Initialize\(\); | 初始化P2P会议类对象，并登陆到穿透服务器。 |  |
|  | WndCreate\(\) | 创建Peergine中间件预览SurfaceView。                         此窗口必须创建，即使APP不需要视频预览或视频播放，都必须创建。因为，P2P中间件需要经过这个窗口的消息队列投递消息到APP的界面里，才成完成回调事件的上报。                              此窗口可以作为视频预览窗口。 |  |
| B |  |  | 开始会议模块 |
|  | Start\(\) | 开始会议 |  |
|  | VideoStart\(\) | 初始化视频模块。 |  |
|  | AudioStart\(\) | 初始化音频模块。 |  |
| C |  |  | 加入会议成员 |
|  | MemberAdd\(\) | 添加会议成员。 |  |
| D |  |  | 视频请求及应答 |
|  | VideoOpen\(\) | 请求或应答视频。 |  |
| E |  |  | 关闭视频 |
|  | VideoClose\(\) | 关闭视频。 |  |
| F |  |  | 停止会议模块 |
|  | AudioStop\(\) | 停止音频模块。 |  |
|  | VideoStop\(\) | 停止视频模块。 |  |
|  | Stop\(\) | 停止会议。 |  |
| G |  |  | 退出清理 |
|  | WndDestroy\(\); | 销毁Peergine中间件窗口。（如果此窗口已经添加到layout中，则需要先从layout删除） |  |
|  | Clean \(\); | 清理P2P会议对象，同时销毁节点对象，并从P2P服务器下线。 |  |




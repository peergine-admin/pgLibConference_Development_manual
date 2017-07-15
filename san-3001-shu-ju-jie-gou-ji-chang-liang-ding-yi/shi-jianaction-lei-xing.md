| Action |  | 说明 |
| :--- | :--- | :--- |
| VideoStatus |  | 视频传输播放状态上报，sData参数的格式为：”bitrate=码率\(bps\)&frmrate=帧率&frmplay=帧号” |
| Message |  | 接收到对端发送的消息，sData参数为消息内容，sPeer参数为对端的节点ID。 |
| Login |  | 本端登录到P2P服务器返回，sData参数返回登录的错误码。 |
| Logout |  | 本端从P2P服务器注销。 |
| AskJoin |  | 请求加入会议。 sPeer：节点名 |
| AskLeave |  | 请求离开会议。 |
| Join |  | 已经加入会议。 |
| Leave |  | 已经离开会议。 |
| VideoSync |  | 视频类同步消息。sPeer：节点名 |
| VideoSyncL |  | 不同流视频类同步消息。sPeer：节点名 |
| VideoOpen |  | 请求打开视频。sPeer：节点名 |
| VideoLost |  | 已经得不到sPeer的视频流了。sPeer：节点名 |
| VideoClose |  | 已经关闭视频。sPeer：节点名 |
| VideoJoin |  | 视频请求端收到打开视频结果通知。 |
| ChairmanSync |  | 主席同步通知。 |
| ChairmanOffline |  | 主席端不在线通知。 |
| PeerSync |  | 同步通知。 |
| PeerOffline |  | 不在线通知。 |
| Notify |  | 收到其他节点群发的消息。sData消息的参数。 |
| SvrNotify |  | 收到P2P服务器下推的消息。sData消息的参数。 |




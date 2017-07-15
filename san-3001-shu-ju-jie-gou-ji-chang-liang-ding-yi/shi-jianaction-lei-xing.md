| Action | 值 | 说明 |
| :--- | :--- | :--- |
| EVENT\_LOGIN | Login | 视频传输播放状态上报，sData参数的格式为：”bitrate=码率\(bps\)&frmrate=帧率&frmplay=帧号” |
| EVENT\_LOGOUT | Logout | 接收到对端发送的消息，sData参数为消息内容，sPeer参数为对端的节点ID。 |
| EVENT\_VIDEO\_LOST | VideoLost | 本端登录到P2P服务器返回，sData参数返回登录的错误码。 |
| EVENT\_AUDIO\_SYNC | AudioSync | 本端从P2P服务器注销。 |
| EVENT\_AUDIO\_CTRL\_VOLUME | AudioCtrlVolume | 请求加入会议。 sPeer：节点名 |
| EVENT\_VIDEO\_SYNC | VideoSync | 请求离开会议。 |
| EVENT\_VIDEO\_SYNC\_1 | VideoSyncL | 已经加入会议。 |
| EVENT\_VIDEO\_OPEN | VideoOpen | 已经离开会议。 |
| EVENT\_VIDEO\_OPEN\_1 | VideoOpenL | 视频类同步消息。sPeer：节点名 |
| EVENT\_VIDEO\_CLOSE | VideoClose | 不同流视频类同步消息。sPeer：节点名 |
| EVENT\_VIDEO\_CLOSE\_1 | VideoCloseL | 请求打开视频。sPeer：节点名 |
| EVENT\_VIDEO\_FRAME\_STAT | VideoFrameStat | 已经得不到sPeer的视频流了。sPeer：节点名 |
| EVENT\_VIDEO\_FRAME\_STAT\_1 | VideoFrameStatL | 已经关闭视频。sPeer：节点名 |
| EVENT\_VIDEO\_JOIN | VideoJoin | 视频请求端收到打开视频结果通知。 |
| EVENT\_VIDEO\_CAMERA | VideoCamera | 主席同步通知。 |
| EVENT\_VIDEO\_RECORD | VideoRecord | 主席端不在线通知。 |
| EVENT\_CHAIRMAN\_SYNC | ChairmanSync | 同步通知。 |
| EVENT\_CHAIRMAN\_OFFLINE | ChairmanOffline | 不在线通知。 |
| EVENT\_PEER\_SYNC | PeerSync | 收到其他节点群发的消息。sData消息的参数。 |
| EVENT\_PEER\_OFFLINE | PeerOffline | 收到P2P服务器下推的消息。sData消息的参数。 |
| EVENT\_ASK\_JOIN | AskJoin |  |
| EVENT\_ASK\_LEAVE | AskLeave |  |
| EVENT\_JOIN | Join |  |
| EVENT\_LEAVE | Leave |  |
| EVENT\_MESSAGE | Message |  |
| EVENT\_NOTIFY | Notify |  |
| EVENT\_SVR\_NOTIFY | SvrNotify |  |
| EVENT\_SVR\_REPLYR\_EEOR | SvrReplyError |  |
| EVENT\_SVR\_RELAY | SvrReply |  |
| EVENT\_CALLSEND\_RESULT | CallSend |  |
| EVENT\_LAN\_SCAN\_RESULT | LanScanResult |  |
|  |  |  |




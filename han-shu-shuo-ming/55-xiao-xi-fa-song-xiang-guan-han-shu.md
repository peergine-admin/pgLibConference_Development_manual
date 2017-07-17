## 5.5 消息发送相关函数

#### MessageSend: 给指定节点发送消息

`/**`

` *  描述：给指定节点发送消息`

` *  阻塞方式：非阻塞，立即返回`

` *  sMsg：[IN] 消息内容`

` *  sPeer：[IN]节点名称`

` *  返回值： true 操作成功，false 操作失败`

` */`

`public boolean MessageSend(String sData, String sPeer)`



#### NotifySend: 给其他所有成员节点发送消息

`/**`

` *  描述：给其他所有成员节点节点发送消息`

` *  阻塞方式：非阻塞，立即返回`

` *  sMsg：[IN] 消息内容`

` *  返回值： true 操作成功，false 操作失败`

` */`

`public boolean NotifySend(String sData)`



`SvrRequest: 给服务器发送消息`

`/**`

` *  描述：给服务器发送消息。`

` *  阻塞方式：非阻塞，立即返回`

` *  返回值： true 操作成功，false 操作失败`

` */`

`public boolean SvrRequest(String sData)`




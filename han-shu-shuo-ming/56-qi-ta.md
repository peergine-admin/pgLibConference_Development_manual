## 5.6 其他



#### SetExpire:设置主席端与成员端的心跳间隔

`/**`

` *  描述：设置主席端与成员端的心跳间隔。`

` *  阻塞方式：非阻塞，立即返回`

` *  iExpire：[IN] 心跳间隔。`

` */`

`public void SetExpire(int iExpire)`



#### SetEventListener: 设置消息接收回调接口 

`/**`

` *  描述：设置消息接收回调接口。`

` *  阻塞方式：非阻塞，立即返回`

` *  eventListener：[IN] 实现了OnEventListner接口的对象，必须定义event函数。`

` */`

`public void SetEventListener(OnEventListener eventListener)`



#### GetNode: 获取自身的pgLibJNINode 类

`/**`

` *  描述：获取自身的pgLibJNINode 类`

` *  阻塞方式：非阻塞，立即返回。`

` *  返回值：自身的pgLibJNINode 类`

` */`

`public pgLibJNINode GetNode()`



#### GetSelfPeer: 获取自身的P2P节点名

`/**`

` *  描述：获取自身的P2P节点名`

` *  阻塞方式：非阻塞，立即返回。`

` *  返回值：自身的P2P节点名`

` */`

`public String GetSelfPeer()`





#### CameraSwitch: 摄像头控制

`/**`

` *  描述：摄像头控制。`

` *  阻塞方式：非阻塞，立即返回`

` *  返回值： true 操作成功，false 操作失败`

` */`

`public boolean CameraSwitch (boolean bEnable)`



#### TimerOutAdd: 将TimerOut接口添加到超时处理列表中

`/**`

` * 描述:将TimerOut接口添加到超时处理列表中。`

` * 阻塞方式：非阻塞`

` * @param timerOut`

` */`

`public void TimerOutAdd(TimerOut timerOut)`



#### TimerOutDel：将TimerOut接口从超时处理列表中删除

`/**`

` * 描述:将TimerOut接口从超时处理列表中删除`

` * 阻塞方式：非阻塞`

` * @param timerOut`

` */`

`public void TimerOutDel(TimerOut timerOut)`



#### TimerStart：开启一个定时器

`/**`

` * 描述：开启一个定时器`

` * 阻塞方式：非阻塞`

` * @param sParam  : 超时处理接口收到的参数`

` * @param iTimeout :超时时间`

` * @param bRepeat : 是否循环`

` * @return  : 定时器实例ID`

` */`

`public int TimerStart(String sParam, int iTimeout, boolean bRepeat)`



#### TimerStop ：关闭一个定时器

`/**`

` * 描述：关闭一个定时器`

` * 阻塞方式：非阻塞`

` * @param iTimerID : 定时器实例ID`

` */`

`public void TimerStop(int iTimerID)`


## 5.2 视频会议控制



#### MemberAdd: 添加成员

`/**`

` *  描述：添加成员（主席端）`

` *  阻塞方式：非阻塞，立即返回`

` *  sMember：[IN] 成员名`

` *  返回值： true 操作成功，false 操作失败`

` */`

`public boolean MemberAdd(String sMember)`



#### MemberDel: 删除成员

`/**`

` *  描述：删除成员（主席端）`

`*  sMember：[IN] 成员名`

` *  阻塞方式：非阻塞，立即返回`

` */`

`public void MemberDel(String sMember)`



#### Join: 请求加入会议

`/**`

` *  描述：请求加入会议（成员端）`

` *  阻塞方式：非阻塞，立即返回`

`*  返回值： true 操作成功，false 操作失败`

` */`

`public boolean Join()`



#### Leave: 离开会议

`/**`

` *  描述：离开会议`

` *  阻塞方式：非阻塞，立即返回`

` */`

`public void Leave()`




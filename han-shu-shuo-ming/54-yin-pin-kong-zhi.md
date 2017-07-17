## 5.4 音频控制



#### AudioStart: 开始播放或采集音频

`/**`

` *  描述：开始播放或采集音频`

` *  阻塞方式：非阻塞，立即返回`

` *   返回值： true 操作成功，false 操作失败`

` */`

`public boolean AudioStart()`



#### AudioStop: 停止播放或采集音频

`/**`

` *  描述：停止播放或采集音频`

` *  阻塞方式：非阻塞，立即返回`

` */`

`public void AudioStop()`

``

#### AudioSpeech: 控制某个节点是否能播放本节点的音频

`/**`

` *  描述：控制某个节点是否能播放本节点的音频。`

` *  阻塞方式：非阻塞，立即返回`

` *  sPeer：节点名`

` *  bEnable: true接收 ，false不接收`

` *  返回值： true 操作成功，false 操作失败`

` */`

`public boolean AudioSpeech(String sPeer, boolean bEnable)`




# 设置群消息已读 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置群消息已读

_**【应用场景】**_

设置群消息已读

注：不提供时间则该UserSysNo在该群的消息全部设置为已读；

_**【接口地址】**_

[http://ip:port/ChatAction/Chat/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etGroupMsgReadedStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 是 | 群系统编码 |
| MsgStartTime | string | 否 | 消息开始时间 |
| MsgEndTime | string | 否 | 消息结束时间 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




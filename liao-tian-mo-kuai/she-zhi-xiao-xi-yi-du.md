# 设置消息已读或点赞等状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置消息已读或点赞等状态

_**【应用场景】**_

设置消息已读或点赞等状态

注：功能1：GroupSysNo+ReadedStatus 可设置群消息全部已读；

功能2：GroupSysNo+MsgSysNo+ReadedStatus 可设置群该条消息已读；

功能3：GroupSysNo+MsgSysNo+SignGoodStatus可设置群该条消息点赞状态；

_**【接口地址】**_

[http://ip:port/ChatAction/Chat/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etGroupMsgStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 是 | 群系统编码 |
| MsgSysNo | int | 否 | 群消息系统编码 |
| ReadedStatus | int | 否 | 设置已读：0否，1是 |
| SignGoodStatus | int | 否 | 是否点赞：0否，1是 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




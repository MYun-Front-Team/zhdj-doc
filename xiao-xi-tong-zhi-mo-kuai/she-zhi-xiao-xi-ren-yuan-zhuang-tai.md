# 设置消息人员状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置消息人员状态

_**【应用场景】**_

设置消息人员状态

注：根据UserSysNo匹配到person，然后根据设置状态，记录该状态的时间；

_**【接口地址】**_

[http://ip:port/MessageAction/Message/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etMessagePersonStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MessageSysNo | int | 是 | 消息系统编码 |
| ReadStatus | int | 是 | 状态：0已发，1已达，10已读 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




# 设置我的群消息通知状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置我的群消息通知状态

_**【应用场景】**_

设置我的群消息通知状态

注：根据UserSysNo，获取Person。

_**【接口地址】**_

[http://ip:port/ChatAction/Chat/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etGroupPersonPushStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 是 | 群系统编码 |
| MsgPushType | int | 是 | 消息通知类型：0全部消息通知，1好友发消息通知，11不通知 |
| JoinPushType | int | 是 | 加入通知类型（管理员默认通知1）：0不通知，1通知 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




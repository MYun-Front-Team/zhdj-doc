# 设置好友申请状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置好友申请状态

_**【应用场景】**_

设置好友申请状态

_**【接口地址】**_

[http://ip:port/ChatAction/Chat/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etFriendJoinStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FriendJoinSysNo | int | 是 | 好友申请系统编码 |
| JoinStatus | int | 是 | 加入状态：0申请中，1加入，2拒绝，3删除 |
| RefuseReason | string | 否 | 拒绝理由 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




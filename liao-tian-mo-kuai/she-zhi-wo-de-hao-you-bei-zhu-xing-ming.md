# 设置我的好友备注姓名 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置我的好友备注姓名

_**【应用场景】**_

设置我的好友备注姓名

_**【接口地址】**_

[http://ip:port/ChatAction/Chat/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etMyFriendPersonName

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 好友人员系统编码 |
| FriendPersonName | string | 否 | 好友备注姓名 |
| FriendStatus | int | 否 | 状态：0正常，11黑名单 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




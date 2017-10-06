# 新增群加入申请 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增群加入申请

_**【应用场景】**_

新增群加入申请

注：当PersonSysNo=0或为空时，表示是自己主动加入群，则通过UserSysNo找到Person。

当PersonSysNo&gt;0时，表示是群管理员邀请，则操作人的UserSysNo找到Person后填入邀请人系统编码中。

_**【接口地址】**_

[http://ip:port/ChatAction/Chat/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddGroupJoin

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 是 | 群系统编码 |
| PersonSysNo | int | 否 | 加入成员系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




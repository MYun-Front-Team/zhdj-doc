# 设置群加入申请状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置群加入申请状态

_**【应用场景】**_

设置群加入申请状态

注：只有管理员权限的成员，才能操作某人的加入申请，并需记录审核人系统编码到表。

_**【接口地址】**_

[http://ip:port/ChatAction/Chat/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etGroupJoinStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupJoinSysNoList | array int | 是 | 群加入申请系统编码列表 |
| JoinStatus | int | 是 | 加入状态：0申请中，1加入，2拒绝 |
| RefuseReason | string | 否 | 拒绝理由 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




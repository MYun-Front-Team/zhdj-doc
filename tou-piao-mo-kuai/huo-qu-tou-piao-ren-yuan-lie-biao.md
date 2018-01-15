# 获取投票人员记录 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取投票人员记录

_**【应用场景】**_

获取投票人员记录

_**【接口地址】**_

[http://ip:port/VoteQuery/Vote/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)VotePersonList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| VoteSysNo | int | 是 | 活动系统编码 |
| LoginIDStatus | array int | 否 | 账号类型：0正常，1无账号，2未激活 |
| Limit |  |  | 限制条件 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

#### VotePersonList说明 {#应答数据-（巡河记录数组）}




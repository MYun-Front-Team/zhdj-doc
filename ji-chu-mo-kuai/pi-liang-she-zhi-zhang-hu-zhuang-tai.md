# 批量设置账户状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置账户状态

_**【应用场景】**_

设置账户状态

注：设置为启用或者禁用；

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etUserListStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| UserSysNoList | array int | 是 | 账户系统编码（原adminSysNo\) |
| UserStatus | int | 是 | 状态：0未激活，1正常，2禁用 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




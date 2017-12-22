# 设置服务商状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置服务商状态

_**【应用场景】**_

设置服务商状态

_**【接口地址】**_

[http://ip:port/OrganizationAction/Servicer/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etServicerStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ServicerSysNo | int | 是 | 系统编码 |
| ServicerStatus | int | 是 | 状态：0待发展，10正常，11终止 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




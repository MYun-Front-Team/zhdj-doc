# 设置坑位状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置坑位状态

_**【应用场景】**_

设置坑位状态

_**【接口地址】**_

[http://ip:port/ShopAction/Hollow/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etHollowStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HollowSysNo | int | 是 | 系统编码 |
| HollowStatus | int | 否 | 状态：10发布，11撤下 |
| IsShield | int | 否 | 是否屏蔽：0否，1是 |
| ShieldReason | string | 否 | 屏蔽理由 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




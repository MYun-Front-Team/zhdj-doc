# 获取积分列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取积分列表

_**【应用场景】**_

获取积分列表

_**【接口地址】**_

[http://ip:port/DMQuery/Party/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)PartyMemberPointsList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DepartmentSysNo | int | 是 | 支部系统编码 |
| MemberName | string | 是 | 姓名 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberSysNo | int | 是 | 党员系统编码 |
| MemberName | string | 是 | 姓名 |
| PartyPost | string | 是 | 党内职务 |
| UserHeadPic | string | 是 | 头像 |




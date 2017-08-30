# 获取党员（风采）列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取党员（风采）列表

_**【应用场景】**_

获取党员（风采）列表

_**【接口地址】**_

[http://ip:port/DMQuery/Party/GetPartyMember](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)s

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberSysNo | int | 否 | 党员系统编码 |
| MemberName | string | 否 | 姓名 |
| CellPhoneNo | string | 否 | 手机 |
| DepartmentSysNo | int | 否 | 所属支部编码 |
| PartyPost | string | 否 | 党内职务 |
| IsShowUser | int | 否 | 是否显示用户 |
| IsShowPoints | int | 否 | 是否显示积分 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberSysNo | int | 是 | 党员编码 |
| DepartmentSysNo | int | 否 | 所属支部编码 |
| MemberName | string | 否 | 姓名 |
| PartyPost | string | 否 | 党内岗位 |
| OrganizationalStatus | int | 否 | 组织状态：0正常，1流动党员 |
| InnerPartyStatus | int | 否 | 党内状态：0入党积极分子，1预备党员，2正式党员 |
| IntroducerSysNo | int |  | 介绍人编码 |
| JoinPartyTime | string | 否 | 入党时间 |
| DuesStandard | decimal | 否 | 党费标准 |
| DuesDate | string | 否 | 党费交至年月 |
| User | object | 否 | 用户实体（见后台接口） |
| PointsValue | int | 否 | 积分值 |




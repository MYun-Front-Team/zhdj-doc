# 获取党员详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取党员详情

_**【应用场景】**_

获取党员详情。

注：当需要获取自己的党员信息时，IsOwner=1，通过UserSysNo匹配到人员后，获取党员信息。

_**【接口地址】**_

[http://ip:port/PartyQuery/Party/GetPartyMember](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)BySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberSysNo | int | 是 | 党员系统编码 |
| IsOwner | int | 否 | 是否获取自己的党员信息（1是） |
| Limit | object | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
|  |  |  | 基本字段 |
|  |  |  | 统计计算字段 |
| Person | object | 是 | Person实体（见登录接口） |

#### LogList说明_ _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LogSysNo | int | 是 | 编码 |
| SourceType | int | 是 | 日志类型 |
| ActionTime | string | 是 | 操作时间 |
| ActionType | int | 是 | 操作动作类型 |
| ActionName | string | 是 | 操作名称 |
| ActionDescription | string | 否 | 操作描述 |




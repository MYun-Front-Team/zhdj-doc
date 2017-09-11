# 获取党员详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取党员详情

_**【应用场景】**_

获取党员详情

_**【接口地址】**_

[http://ip:port/PartyQuery/Party/GetPartyMember](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)BySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberSysNo | int | 是 | 党员系统编码 |
| Limit | object | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
|  |  |  | 基本字段 |
|  |  |  | 统计计算字段 |

#### LogList说明_ _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LogSysNo | int | 是 | 编码 |
| SourceType | int | 是 | 日志类型 |
| ActionTime | string | 是 | 操作时间 |
| ActionType | int | 是 | 操作动作类型 |
| ActionName | string | 是 | 操作名称 |
| ActionDescription | string | 否 | 操作描述 |




# 获取支部党员党费缴纳列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取支部党员党费缴纳列表

_**【应用场景】**_

获取支部党员党费缴纳列表

_**【接口地址】**_

[http://ip:port/PartyQuery/Party/GetPartyBranch](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)FeeList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 支部系统编码 |
| FeeYear | int | 是 | 缴费年份（如2017） |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PartyMemberSysNo | int | 是 | 党员系统编码 |
| Person | object | 是 | 党员人员简要实体 |
| DuesStandard | decimal\(18,2\) | 是 | 缴费标准（元/月） |
|  |  |  |  |
| TotalFee | decimal\(18,2\) | 是 | 应缴纳费用 |
| PaidFee | decimal\(18,2\) | 是 | 已缴纳费用 |
| LeftFee | decimal\(18,2\) | 是 | 待缴纳费用 |
| MonthFeeList | array object | 是 | 月缴纳费用列表 |

#### MonthFeeList说明_ _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeMonth | int | 是 | 缴纳月份（如2） |
| DuesStandard | decimal\(18,2\) | 是 | 缴纳费用 |
| FeeStatus | int | 是 | 状态：0未缴，1已缴 |
| CreatePersonName | string | 是 | 操作人姓名 |
| CreateDate | string | 是 | 操作时间 |




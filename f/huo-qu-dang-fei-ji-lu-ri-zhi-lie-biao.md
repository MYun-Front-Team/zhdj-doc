# 获取党费记录日志列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取党费记录日志列表

_**【应用场景】**_

获取党费记录日志列表

_**【接口地址】**_

[http://ip:port/PartyQuery/Party/GetP](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)artyFeeList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PartyMemberSysNo | int | 是 | 党员系统编码 |
| FeeStatusList | array int | 否 | 状态列表：0待确认，1待支付，10有效，11无效 |
| IsReceivedList | array int | 否 | 线上支付是否已经到账管理人微信、银行卡里|


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeLogSysNo | int | 是 | 系统编码 |
| Fee | decimal\(18,2\) | 是 | 金额 |
| DuesStandard | decimal\(18,2\) | 是 | 缴费标准（元/月） |
| FeeStartDate | string | 是 | 开始年月 |
| FeeEndDate | string | 是 | 结束年月 |
| Remark | string | 否 | 备注 |
| FeeStatus | int | 是 | 状态：0待确认，10有效，11无效 |
| CreatePersonName | string | 是 | 录入人姓名 |
| RemoveReason | string | 否 | 作废原因 |
| RemovePersonName | string | 否 | 作废人姓名 |
| RemoveTime | string | 否 | 作废时间 |
| IsReceived| int | 是 | 线上支付是否已经到账管理人微信、银行卡里|


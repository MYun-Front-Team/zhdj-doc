# 确认党费记录状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

确认党费记录状态

_**【应用场景】**_

确认党费记录状态

注：FeeStatus必须是：10有效，11无效；

注：如果确认有效，记录到党员模块的党费日志表，并更新党员表的最后缴费年月；

_**【接口地址】**_

[http://ip:port/PartyAction/Party/SetP](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)artyFeeStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeLogSysNo | int | 是 | 党费记录日志系统编码 |
| Fee | decimal\(18,2\) | 是 | 金额 |
| DuesStandard | decimal\(18,2\) | 是 | 缴费标准（元/月） |
| FeeStartDate | string | 是 | 开始年月 |
| FeeEndDate | string | 是 | 结束年月 |
| Remark | string | 否 | 备注 |
| FeeStatus | int | 是 | 状态：10有效，11无效 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




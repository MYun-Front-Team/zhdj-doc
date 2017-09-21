# 新增党费记录 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增党费记录

_**【应用场景】**_

新增党费记录

注：存入通用日志表，并更新党员表的最后缴费年月。（见日志枚举说明）

_**【接口地址】**_

[http://ip:port/PartyAction/Party/AddP](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)artyFee

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PartyMemberSysNo | int | 是 | 党员系统编码 |
| Fee | int | 是 | 金额 |
| FeeStartDate | string | 是 | 开始年月 |
| FeeEndDate | string | 是 | 结束年月 |
| Remark | string | 否 | 备注 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SysNo | int | 是 | 系统编码 |




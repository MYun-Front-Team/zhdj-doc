# 获取超额预警列表

##### _【功能说明】_ {#【功能说明】}

获取超额预警列表

_**【应用场景】**_

平台基础数据报表

_**【接口地址】**_

[http://ip:port/RecruitQuery/Wallet/GetWageExcessList]
(http://ip:port/RecruitQuery/Wallet/GetWageExcessList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WageMonth| datetime| 是 | 发放月份 |
| Keyword| string | 是 | 关键字（姓名或手机号） |


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CustomerName| string | 是 | 姓名|
| CellPhone| string | 是 | 手机号|
| WageMonth| datetime| 是 | 发放月份 |
| WageAmount | decimal（18，2） | 是 | 月累计发放金额 |
| ExcessAmount | decimal（18，2） | 是 | 月累计发放金额 |





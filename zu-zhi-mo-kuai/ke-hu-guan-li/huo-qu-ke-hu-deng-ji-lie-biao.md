# 获取客户等级列表 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

获取客户等级列表

_**【应用场景】**_

获取客户等级列表

_**【接口地址】**_

[http://ip:port/OrganizationQuery/CustomerLevel/GetCustomer](http://ip:port/OrganizationAction/Customer/AddCustomer)LevelList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |

#### _应答数据 _ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CustomerLevelSysNo | int | 是 | 系统编码 |
| CustomerLevelName | string | 是 | 客户等级名称 |
| OwnConsumeAmount | decimal\(18,2\) | 否 | 满足自己消费金额 |
| InvitingConsumeAmount | decimal\(18,2\) | 否 | 满足邀请消费金额 |
| ProfitRateList | array decimal\(18,4\) | 否 | 分享比率列表（按排序） |
| DiscountRate|  decimal（18,4) | 否 | 折扣 (0-1)|
| Remark|  string | 否 |描述 |





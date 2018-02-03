# 获取商家等级列表 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

获取商家等级列表

_**【应用场景】**_

获取商家等级列表

_**【接口地址】**_

[http://ip:port/OrganizationQuery/SellerLevel/GetSeller](http://ip:port/OrganizationAction/Customer/AddCustomer)LevelList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |

#### _应答数据 （数组）_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SellerLevelSysNo | int | 是 | 系统编码 |
| SellerLevelName | string | 是 | 商家等级名称 |
| TotalMemberShipFee | decimal\(18,2\) | 否 | 累计缴纳会员费 |
| TotalCustomerCount | int | 否 | 累计推广客户数 |




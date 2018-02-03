# 新增商家等级 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增商家等级

_**【应用场景】**_

新增商家等级

注：如果累计的值为空，则数据库存一个无穷大的值；

_**【接口地址】**_

[http://ip:port/OrganizationAction/SellerLevel/AddS](http://ip:port/OrganizationAction/Customer/AddCustomer)ellerLevel

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| SellerLevelName | string | 是 | 商家等级名称 |
| TotalMemberShipFee | decimal\(18,2\) | 否 | 累计缴纳会员费 |
| TotalCustomerCount | int | 否 | 累计推广客户数 |

#### _应答数据 _ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SellerLevelSysNo | int | 是 | 系统编码 |




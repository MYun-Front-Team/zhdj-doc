# 修改客户 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改客户

_**【应用场景】**_

修改客户

_**【接口地址】**_

[http://ip:port/OrganizationAction/Customer/EditCustomer](http://ip:port/OrganizationAction/Customer/AddCustomer)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CustomerSysNo | int | 是 | 客户系统编码 |
| CustomerLevelSysNo | int | 否（可选配置） | 客户等级系统编码 |
| CustomerStatus | int | 否（可选配置） | 状态：0待发展，10正常，11终止 |
| CustomerName | string | 否 | 客户名称 |
| CustomerShortName | string | 否（可选配置） | 简称 |
| CustomerTel | string | 否（可选配置） | 客户联系电话 |
| CustomerDesc | string | 否（可选配置） | 客户描述 |
| CustomerMaster | string | 否（可选配置） | 客户负责人 |
| CustomerPost | string | 否（可选配置） | 客户负责人岗位 |
| CustomerPerson | string | 否（可选配置） | 客户联系人 |
| CustomerPersonPhone | string | 否（可选配置） | 客户联系人电话 |
| CustomerPersonPost | string | 否（可选配置） | 客户联系人岗位 |
| ContractAddress | string | 否（可选配置） | 联系地址 |
| Longitude | decimal\(18,2\) | 否 | 经度 |
| Latitude | decimal\(18,2\) | 否 | 纬度 |

#### _应答数据 _ {#应答数据-}




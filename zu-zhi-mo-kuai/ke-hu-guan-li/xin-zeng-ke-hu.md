# 新增客户 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增客户

_**【应用场景】**_

新增客户

注：OrganizationToSysNo可以为0

_**【接口地址】**_

[http://ip:port/OrganizationAction/Customer/AddCustomer](http://ip:port/OrganizationAction/Customer/AddCustomer)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| OrganizationToSysNo | int | 否（可选配置） | 客户方组织系统编码 |
| CustomerLevelSysNo | int | 否（可选配置） | 客户等级系统编码 |
| CustomerStatus | int | 否（可选配置） | 状态：0待发展，10正常，11终止 |
| CustomerName | string | 是 | 客户名称 |
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
| CustomerLogoPathList | array string | 否（可选配置） | 客户Logo的路径列表 |
| IsPartner| int | 是 |是否合伙人|




#### _应答数据 _ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CustomerSysNo | int | 是 | 系统编码 |




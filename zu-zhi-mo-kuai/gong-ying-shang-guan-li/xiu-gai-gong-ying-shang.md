# 修改供应商 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改供应商

_**【应用场景】**_

修改供应商

_**【接口地址】**_

[http://ip:port/OrganizationAction/Supplier/EditS](http://ip:port/OrganizationAction/Customer/AddCustomer)upplier

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SupplierSysNo | int | 是 | 供应商系统编码 |
| SupplierLevelSysNo | int | 否（可选配置） | 供应商等级系统编码 |
| SupplierStatus | int | 否（可选配置） | 状态：0待发展，10正常，11终止 |
| SupplierName | string | 否 | 供应商名称 |
| SupplierShortName | string | 否（可选配置） | 简称 |
| SupplierTel | string | 否（可选配置） | 供应商联系电话 |
| SupplierDesc | string | 否（可选配置） | 供应商描述 |
| SupplierMaster | string | 否（可选配置） | 供应商负责人 |
| SupplierPost | string | 否（可选配置） | 供应商负责人岗位 |
| SupplierPerson | string | 否（可选配置） | 供应商联系人 |
| SupplierPersonPhone | string | 否（可选配置） | 供应商联系人电话 |
| SupplierPersonPost | string | 否（可选配置） | 供应商联系人岗位 |
| ContractAddress | string | 否（可选配置） | 联系地址 |
| Longitude | decimal\(18,2\) | 否 | 经度 |
| Latitude | decimal\(18,2\) | 否 | 纬度 |
| SupplierLogoPathList | array string | 否（可选配置） | 供应商Logo的路径列表 |
| Remark1| string | 否 | 备注1 |
| Remark2| string | 否 | 备注2 |



#### _应答数据 _ {#应答数据-}




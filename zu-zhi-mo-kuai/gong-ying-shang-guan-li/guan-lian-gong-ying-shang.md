# 关联供应商 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

关联供应商

_**【应用场景】**_

关联供应商

注：1、先判断供应商组织是否已经是我的供应商，如果不存在则新增，不抛错；

2、判断该供应商组织是否是合法的商家；

_**【接口地址】**_

[http://ip:port/OrganizationAction/Supplier/SetS](http://ip:port/OrganizationAction/Customer/AddCustomer)upplierRelation

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationFromSysNo | int | 是 | 组织系统编码 |
| OrganizationToSysNo | int | 是 | 供应商方组织系统编码 |

#### _应答数据 _ {#应答数据-}




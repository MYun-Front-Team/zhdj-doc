
#启用/禁用商家

##### _【功能说明】_ {#【功能说明】}

启用/禁用商家

_**【应用场景】**_

启用/禁用商家


_**【接口地址】**_

http://ip:port/OrganizationAction/Seller/SetSellerIsDisable

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SellerSysNo | int | 否 | 商家系统编码(和组织系统编码2传1) |
| OrganizationSysNo | int | 否 | 组织系统编码(和商家系统编码2传1)  |
|IsDisable| int | 否 |是否禁用（1禁用，0启用）|



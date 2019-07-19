# 修改客户经理 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改客户经理

_**【应用场景】**_

_**【接口地址】**_

http://ip:port/OrganizationAction/CustomerManager/EditCustomerManager

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CustomerManagerSysNo | int | 是 | 系统编码 |
| ManagerName | string | 是 | 客户经理名称 |
| ManagerType| int | 否 | 类型（1-经理2-顾问3-业务员）|
| CellPhoneNo| string| 否 | 手机号 |


#### _应答数据 _ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CustomerManagerSysNo | int | 是 | 系统编码 |




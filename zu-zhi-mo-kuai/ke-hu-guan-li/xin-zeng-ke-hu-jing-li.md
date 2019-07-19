# 新增客户经理 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增客户等级

_**【应用场景】**_

新增客户等级

_**【接口地址】**_

http://ip:port/OrganizationAction/CustomerManager/AddCustomerManager

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ManagerName | string | 是 | 客户经理名称 |
| ManagerType| int | 否 | 类型（1-经理2-顾问3-业务员）|
| CellPhoneNo| string| 否 | 手机号 |
| LoginID|string  | 是 | 登录账号 |
| LoginPassword|string  | 是 | 登录密码 |




#### _应答数据 _ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CustomerManagerSysNo | int | 是 | 系统编码 |




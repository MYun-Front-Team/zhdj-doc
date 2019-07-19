# 获取客户经理/顾问列表
##### _【功能说明】_ {#【功能说明】}

获取客户经理/顾问列表

_**【应用场景】**_

获取客户经理/顾问列表

_**【接口地址】**_

http://ip:port/OrganizationQuery/Customer/GetCustomerManagerList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ManagerType| int | 否 |类型（1顾问 2经理）|
| KeyWord| strig | 否 |业务员姓名、手机号|
| ManagerStatusList| List<int> | 否 |状态（0待激活10已启用11已禁用）|




> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ManagerName| string | 否 |顾问名称|
| ManagerType| int | 否 |类型（1顾问 2经理）|
| ManagerSysNo| int | 否 |顾问系统编码|
| ManagerStatus| int | 否 |状态（0待激活10已启用11已禁用）|
| CellPhoneNo| string | 否 |手机号|
|CustomerCount| int | 否 |负责客户数|
|LastLoginTime| string| 否 |最近登录时间|








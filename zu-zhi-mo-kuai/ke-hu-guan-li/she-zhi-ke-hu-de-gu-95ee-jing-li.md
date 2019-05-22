# 设置客户的顾问/经理

##### _【功能说明】_ {#【功能说明】}

设置客户的顾问/经理

_**【应用场景】**_
设置客户的顾问/经理

_**【接口地址】**_

http://ip:port/OrganizationAction/Customer/CustomerSetManager

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CustomerSysNoList | Array[int] | 是 | 客户系统编码 |
| ManagerType| int | 否 |类型（1顾问 2经理）|
| ManagerSysNoList| Array[int]  | 否 |顾问系统编码|

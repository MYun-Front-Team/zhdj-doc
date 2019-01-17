# 获取服务人员列表

_**【接口地址】**_

http://ip:port/FJQuery/Adaption/GetServicePersonList

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonName | string | 否 | 姓名 |
| AreaCode | string | 否 | 区域编号 |
| EnableList | array int | 否 | 1启用，2禁用 |

> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员id |
| AdminSysNo | int | 是 | 账户编码 |
| LoginId | string | 是 | 登录账号 |
| PersonName | string | 是 | 用户姓名 |
| CellPhoneNo | string | 否 | 手机号 |
| UserGender | int | 否 | 1男，2女 |
| Email | string | 否 | 邮箱 |
| AreaCode | string | 是 | 区域编号 |
| AreaName | string | 是 | 区域名称 |

| DepartmentSysNo | int | 是 | 部门id |
| IsEnable | int | 是 | 1启用，2禁用 |









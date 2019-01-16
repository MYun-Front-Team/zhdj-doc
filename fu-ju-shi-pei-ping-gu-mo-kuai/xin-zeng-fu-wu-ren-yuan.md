# 新增服务人员

_**【接口地址】**_

http://ip:port/FJAction/Adaption/AddServicePerson

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LoginId | string | 是 | 登录账号 |
| LoginPwd | string | 是 | 登录密码 |
| PersonName | string | 是 | 用户姓名 |
| CellPhoneNo | string | 否 | 手机号 |
| UserGender | int | 否 | 1男，2女 |
| Email | string | 否 | 邮箱 |
| AreaCode | string | 是 | 区域编号 |
| DepartmentSysNo | int | 是 | 部门id |

> #### _应答数据_


| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 人员id |


LoginSource 1
LoginType 4
OrganizationType  17041





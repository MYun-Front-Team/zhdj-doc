# 新增管理员

_**【接口地址】**_

http://ip:port/FJAction/Adaption/AddAdminPerson

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LoginId | string | 是 | 登录账号 |
| LoginPwd | string | 是 | 登录密码 |
| PersonName | string | 是 | 用户姓名 |
| CellPhoneNo | string | 否 | 手机号 |
| AreaCode | string | 是 | 区域编号 |
| DepartmentSysNo | int | 是 | 部门id |
| PostSysNo | int | 是 | 岗位id |

> #### _应答数据_


| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 人员id |


LoginSource 2
LoginType 4
OrganizationType  17042








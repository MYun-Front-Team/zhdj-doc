# 获取管理员列表

_**【接口地址】**_

http://ip:port/FJQuery/Adaption/GetAdminPersonList

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
| LoginId | string | 是 | 登录账号 |
| LoginPwd | string | 是 | 登录密码 |
| PersonName | string | 是 | 用户姓名 |
| CellPhoneNo | string | 否 | 手机号 |
| AreaCode | string | 是 | 区域编号 |
| DepartmentSysNo | int | 是 | 部门id |
| PostSysNo | int | 是 | 岗位id |









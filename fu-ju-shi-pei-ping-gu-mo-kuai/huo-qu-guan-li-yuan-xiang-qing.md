# 获取管理员详情

_**【接口地址】**_

http://ip:port/FJQuery/Adaption/GetAdminPersonBySysNo

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员id |

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
| RightList | array Right | 是 | 权限列表 |

Right

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RightSysNo | int | 是 | 权限系统编码 |
| RightName | string | 是 | 权限名称 |
| RightCode | string | 是 | 权限代码 |
| RightType | int | 是 | 权限类型：1模块，2子模块，3页面，4按钮 |



















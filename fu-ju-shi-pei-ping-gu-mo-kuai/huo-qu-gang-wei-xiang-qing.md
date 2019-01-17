# 获取岗位详情

_**【接口地址】**_

http://ip:port/FJQuery/Adaption/GetPostBySysNo

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PostSysNo | int | 是 | 岗位id |

> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PostSysNo | int | 是 | 岗位id |
| Name | string | 是 | 岗位名称 |
| DepartmentSysNo | int | 是 | 部门id |
| Department | string | 是 | 部门名称 |
| Master | string | 是 | 负责人 |
| AreaCode | string | 是 | 区域编号 |
| AreaName | string | 是 | 区域名称 |
| IsEnable | int | 是 | 1启用，0禁用 |
| RightList | array Right | 是 | 权限列表 |

Right

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RightSysNo | int | 是 | 权限系统编码 |
| RightName | string | 是 | 权限名称 |
| RightCode | string | 是 | 权限代码 |
| RightType | int | 是 | 权限类型：1模块，2子模块，3页面，4按钮 |










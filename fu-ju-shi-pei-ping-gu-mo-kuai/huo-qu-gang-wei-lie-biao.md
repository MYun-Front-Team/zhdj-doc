# 获取岗位列表

_**【接口地址】**_

http://ip:port/FJQuery/Adaption/GetPostList

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Name | string | 否 | 岗位名称 |

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









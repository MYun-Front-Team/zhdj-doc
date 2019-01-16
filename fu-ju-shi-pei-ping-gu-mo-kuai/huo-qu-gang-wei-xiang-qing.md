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
| IsEnable | int | 是 | 1启用，0禁用 |









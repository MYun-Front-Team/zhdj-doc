# 新增岗位

_**【接口地址】**_

http://ip:port/FJAction/Adaption/AddPost

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Name | string | 是 | 岗位名称 |
| DepartmentSysNo | int | 是 | 部门id |
| Master | string | 是 | 负责人 |
| AreaCode | string | 是 | 区域编号 |
| RightList | array int | 否 | 权限列表 |

> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 岗位id |









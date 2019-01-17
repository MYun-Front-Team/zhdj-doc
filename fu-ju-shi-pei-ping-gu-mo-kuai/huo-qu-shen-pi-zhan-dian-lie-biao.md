# 获取审批站点列表

_**【接口地址】**_

http://ip:port/FJQuery/Adaption/GetApproveNodeList

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AreaCode | string | 否 | 区域编号 |

> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ApproveNodeSysNo | int | 是 | 审批节点id |
| ApproveType | int | 是 | 5村社区，4乡镇街道，3区县，2市级，1省级 |
| AreaCode | string | 是 | 区域编号 |
| AreaName | string | 是 | 区域名称 |
| DepartmentSysNo | int | 是 | 部门id |
| Department | string | 是 | 部门 |
| PostSysNo | int | 是 | 岗位id |
| Post | string | 是 | 岗位 |
| NeedAssess | int | 是 | 1需要评估，0不需要评估 |

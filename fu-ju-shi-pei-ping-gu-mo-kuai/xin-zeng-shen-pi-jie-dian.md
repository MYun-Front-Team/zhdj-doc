# 新增审批节点

_**【接口地址】**_

http://ip:port/FJAction/Adaption/AddApproveNode

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ApproveType | int | 是 | 5村社区，4乡镇街道，3区县，2市级，1省级 |
| AreaCode | string | 是 | 区域编号 |
| DepartmentSysNo | int | 是 | 部门id |
| PostSysNo | int | 是 | 岗位id |
| NeedAssess | int | 是 | 1需要评估，0不需要评估 |


> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 审批节点id |

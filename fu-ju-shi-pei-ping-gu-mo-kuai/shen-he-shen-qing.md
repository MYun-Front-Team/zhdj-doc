# 审核申请

_**【接口地址】**_

http://ip:port/FJAction/Adaption/ApproveApply

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ApplySysNo | int | 是 | 申请id |
| ApprovePersonSysNo | int | 是 | 审核人编码 |
| ApproveType | int | 是 | 10通过，11拒绝 |
| ApproveRemark | string | 是 | 审批意见 |

> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |

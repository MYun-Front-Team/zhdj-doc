# 设置审核状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置审核状态

_**【应用场景】**_

设置审核状态

注：提交审核时，原因可以为空，审核通过或者失败时，原因必填；

记录Log日志，详情内需要展示；

_**【接口地址】**_

[http://ip:port/StudentFeeAction/StudentFee/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etStudentFeeAuditStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentFeeSysNo | int | 是 | 缴费系统编码 |
| AuditStatus | int | 是 | 审核状态：0未提交，1审核中，10审核通过，11审核失败 |
| Reason | string | 否 | 原因 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




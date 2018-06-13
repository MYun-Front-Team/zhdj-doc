# 设置缴费状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置缴费状态

_**【应用场景】**_

设置缴费状态

注：审核通过的缴费记录才允许设置缴费状态；

记录操作日志（重要）；

_**【接口地址】**_

[http://ip:port/StudentFeeAction/StudentFee/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etStudentFeePaidStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentFeeSysNo | int | 是 | 缴费系统编码 |
| PaidStatus | int | 是 | 缴费状态：0未开始缴费，1未下载，2已下载 9缴费中，10缴费完成 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




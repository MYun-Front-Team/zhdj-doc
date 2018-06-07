# 导入禾城报表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

导入禾城报表

_**【应用场景】**_

导入禾城报表 

注：审核通过且缴费中状态的记录才允许导入禾城报表；

每次导入可覆盖之前的记录；

记录操作日志（重要）；

_**【接口地址】**_

[http://ip:port/StudentFeeAction/StudentFee/I](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)mportStudentFeeRecordList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentFeePersonSysNo | int | 是 | 缴费系统明细编码 |
| Remark| string| 是 |备注|
| PaidAmount| decimal| 是 |实际缴费|
| PaidTime| decimal| 是 |记账日期|




> #### _应答数据 _ {#应答数据-（巡河记录数组）}




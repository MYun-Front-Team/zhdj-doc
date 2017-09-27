# 删除党费记录 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

删除党费记录

_**【应用场景】**_

删除党费记录

注：党费日志表设置FeeStatus=11并记录作废操作人RemoveUserSysNo，并更新党员表的最后缴费年月。

_**【接口地址】**_

[http://ip:port/PartyAction/Party/DeleteP](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)artyFee

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeLogSysNo | int | 是 | 系统编码 |
| RemoveReason | string | 是 | 作废原因 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




# 获取工单回复流转列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取工单回复流转列表

_**【应用场景】**_

获取工单回复流转列表

_**【接口地址】**_

[http://ip:port/WorkQuery/Work/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)WorkReplyList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WorkSysNo | int | 是 |  |
| ReplyTypeList | array int | 否 | 限制条件 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WorkBase | object | 是 | 基础字段 |
| WorkStatistic | object | 否 | 统计字段 |




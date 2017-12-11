# 获取工单详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取工单详情

_**【应用场景】**_

获取工单详情

注：Limit中IsShowReplyList只显示回复状态为ReplyType=0的列表数据；

_**【接口地址】**_

[http://ip:port/WorkQuery/Work/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)WorkBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WorkSysNo | int | 是 | 系统编码 |
| ReplyTypeList | array int | 否 | 回复类型：0回复，1流转 |
| Limit | array | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WorkBase | object | 是 | 基础字段 |
| WorkStatistic | object | 否 | 统计字段 |




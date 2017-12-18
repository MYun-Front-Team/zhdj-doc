# 获取工单统计 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取工单统计

_**【应用场景】**_

获取工单统计

_**【接口地址】**_

[http://ip:port/WorkQuery/Work/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)WorkStatistics

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Query | object | 是 | 见搜索条件 |
| Limit | array | 否 | 限制条件 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Score | decimal\(18,2\) | 是 | 评分 |
| WorkStatisticList | array object | 是 | 统计数量数组 |

#### WorkStatistic说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WorkStatus | int | 是 | 工单状态 |
| WorkCount | int | 是 | 数量 |




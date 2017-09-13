# 获取活动详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取活动详情

_**【应用场景】**_

获取活动详情。

注意：如该人未曾阅读，插入一条人员足迹，标记已读。

_**【接口地址】**_

[http://ip:port/ActivityQuery/Activity/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ActivityBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivitySysNo | int | 否 | 系统编码 |
| Limit | array | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivityBase | object | 是 | 基础字段 |
| ActivityStatistic | object  | 否 | 统计字段 |



####  {#应答数据-（巡河记录数组）}




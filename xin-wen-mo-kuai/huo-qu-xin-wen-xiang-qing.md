# 获取新闻详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取新闻详情

_**【应用场景】**_

获取新闻详情。

注意：判断该人是否已经浏览过，是则累计浏览次数，否则新增。

积分备注：浏览动作（枚举=3）预埋积分赠送逻辑。

_**【接口地址】**_

[http://ip:port/NewsQuery/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[News](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[News](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)BySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| NewsSysNo | int | 否 | 系统编码 |
| Limit | array | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| NewsBase | object | 是 | 基础字段 |
| NewsStatistic | object | 否 | 统计字段 |




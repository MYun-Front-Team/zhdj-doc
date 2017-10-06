# 获取推荐群列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取推荐群列表

_**【应用场景】**_

获取推荐群列表

_**【接口地址】**_

[http://ip:port/ChatQuery/Chat/G](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etRecommendGroupList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupClassSysNo | int | 是 | 群分类系统编码（类别树） |
| Limit | object | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupBase | object | 是 | 基础字段 |
| GroupStatistic | object | 否 | 计算字段 |




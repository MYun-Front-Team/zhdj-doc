# 获取商品推荐列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取商品推荐列表

_**【应用场景】**_

获取商品推荐列表

注：一旦启用“IsShowHollowTime”，那么商品必须为上架状态；

_**【接口地址】**_

[http://ip:port/ShopQuery/Recommend/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)RecommendList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Query | object | 是 | 搜索条件 |
| Limit | object | 否 | 限制条件 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecommendBase | object | 是 | 基础字段 |
| RecommendStatistic | object | 否 | 统计字段 |




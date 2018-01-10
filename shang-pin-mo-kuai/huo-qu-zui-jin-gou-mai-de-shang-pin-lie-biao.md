# 获取最近购买的商品列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取最近购买的商品列表

_**【应用场景】**_

获取最近购买的商品列表

注：如果组织编码为空，那么根据UserSysNo来查询组织；

_**【接口地址】**_

[http://ip:port/ProductQuery/ProductGroup/GetBoughtProductGroupList](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 组织系统编码 |
| Limit | array | 否 | 限制条件 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupBase | object | 是 | 基础字段 |
| ProductGroupStatistic | object | 否 | 统计字段 |




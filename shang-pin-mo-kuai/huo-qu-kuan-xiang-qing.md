# 获取款详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取款详情

_**【应用场景】**_

获取款详情

注：当DataRangeSysNo=0时，查询该商品所属组织的详情，否则则为该店铺的详情；

_**【接口地址】**_

[http://ip:port/ProductQuery/ProductGroup/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ProductGroupBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围结点（店铺树） |
| ProductGroupSysNo | int | 是 | 款系统编码 |
| Limit | array | 否 | 限制条件 |
| TouristOrganizationSysNo | int | 是 | 游客组织系统编码（传0即为游客） |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupBase | object | 是 | 基础字段 |
| ProductGroupStatistic | object | 否 | 统计字段 |




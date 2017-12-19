# 获取商家详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取商家详情

_**【应用场景】**_

获取商家详情

注：

_**【接口地址】**_

[http://ip:port/OrganizationQuery/Seller/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)SellerBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否（二选一必须） | 组织系统编码 |
| SellerSysNo | int | 否（二选一必须） | 商家系统编码 |
| Limit | array | 否 | 限制条件 |

> #### _应答数据_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SellerBase | object | 是 | 基础字段 |
| SellerStatistic | object | 否 | 统计字段 |




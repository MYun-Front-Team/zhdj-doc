# 获取商品推荐栏目详情

##### _【功能说明】_ {#【功能说明】}

获取商品推荐栏目详情

_**【应用场景】**_

获取商品推荐栏目详情


_**【接口地址】**_

http://ip:port/ShopQuery/Recommend/GetRecommendTypeBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecommendTypeSysNo | int | 否 | 所有者组织系统编码 |




> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecommendTypeSysNo | int | 是 | 栏目系统编码 |
| OrganizationSysNo | int | 是 | 所有者组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围系统编码（店铺树） |
| RecommendTypeName | string| 是 | 栏目名称 |






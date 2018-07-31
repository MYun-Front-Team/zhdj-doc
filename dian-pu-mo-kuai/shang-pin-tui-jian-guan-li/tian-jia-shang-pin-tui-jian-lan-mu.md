# 添加商品推荐栏目

##### _【功能说明】_ {#【功能说明】}

添加商品推荐栏目

_**【应用场景】**_

添加商品推荐栏目

_**【接口地址】**_

http://ip:port/ShopAction/Recommend/AddRecommendType
> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 所有者组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围系统编码（店铺树） |
| RecommendTypeName | string| 是 | 栏目名称 |


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecommendTypeSysNo | int | 是 | 系统编码 |




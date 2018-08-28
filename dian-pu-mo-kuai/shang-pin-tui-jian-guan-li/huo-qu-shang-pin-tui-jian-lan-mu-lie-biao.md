# 获取商品推荐栏目列表

##### _【功能说明】_ {#【功能说明】}

获取商品推荐栏目列表

_**【应用场景】**_

获取商品推荐栏目列表


_**【接口地址】**_

http://ip:port/ShopQuery/Recommend/GetRecommendTypeList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 所有者组织系统编码 |
| DataRangeSysNoList | array int | 否 | 数据范围系统编码（投放位置树） |
| KeyWord | string| 是 | 关键字 |



> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecommendTypeSysNo | int | 是 | 栏目系统编码 |
| OrganizationSysNo | int | 是 | 所有者组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围系统编码（店铺树） |
| RecommendTypeName | string| 是 | 栏目名称 |
| RecommendTypePathList | array string | 否 | 栏目主图path路径 |
| RecommendTypeUrlList | array string | 否 | 栏目主图url路径 |
| Remark| string| 是 | 栏目备注 |












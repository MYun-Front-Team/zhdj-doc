#获取同款商品列表

##### _【功能说明】_ {#【功能说明】}

获取同款商品列表

_**【应用场景】**_

获取同款商品列表

_**【接口地址】**_

http://ip:port/ProductQuery/ProductGroup/GetGroupByProduct


> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupByCode| string| 否 | 多款聚合款号 |
| IsOneBuy| int | 是 | 是否是一元购入口进入 |



> #### 返回数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo| int | 是 | 款系统编码 |
| OrganizationSysNo|int| 是 |组织系统编码|
| GroupByCode| string| 否 | 多款聚合款号 |
| GroupByOtherName| string| 否 | 多款聚合别名 |










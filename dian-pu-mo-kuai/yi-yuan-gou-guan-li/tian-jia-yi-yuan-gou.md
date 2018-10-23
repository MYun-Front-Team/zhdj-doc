
# 添加一元购

##### _【功能说明】_ {#【功能说明】}

添加一元购

_**【应用场景】**_

添加一元购

_**【接口地址】**_

http://ip:port/ShopAction/OneBuy/AddOneBuy


> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo| int | 是 |平台编码 |
| DataRangeSysNo| int | 是 |店铺范围编码 |
| ProductGroupList|array[ProductGroup] | 是 |款编码范围编码 |
| StartTime| datetime | 是 | 开始时间 |
| EndTime| int | 是 | 结束时间 |




> #### ProductGroup

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo|int | 是 |款编码范围编码 |
| FakeSaleCount| int | 是 |已经购买|
| FakeInventoryCount| int | 是 |总份数|
| SalePrice | decimal\(18,2\) | 否 | 必砍价 |






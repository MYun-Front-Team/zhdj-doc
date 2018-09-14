# 获取一元购列表

##### _【功能说明】_ {#【功能说明】}

获取一元购列表

_**【应用场景】**_

获取一元购列表

_**【接口地址】**_

http://ip:port/ShopQuery/OneBuy/GetOneBuyList


> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupClassSysNoList | array int | 否 | 类型分类系统编码（类别树） |
| OneBuyStatusList | array int | 否 |有效状态 0未开始，10进行中，11已结束 |
| KeyWord| string | 否 |关键字|





> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OneBuySysNo| int| 是 |系统编码|
| SourceProductGroupCode| string| 否 | 引入商品编码 |
| FileThumbnailUrlList | array string | 否 | 缩略图Path列表（第一张为首图） |
| ProductGroupName| string| 否 | 商品名称|
| ProductGroupClassName | string | 否 | 分类名称（类别树） |
| CPSCommissionRate|decimal| 是 | CPS佣金比率|
| SalePrice | decimal\(18,2\) | 否 | 销售价 |
| OnSaleStatus| int | 是 | 上下架 |
| StartTime| datetime | 是 | 开始时间 |
| EndTime| int | 是 | 结束时间 |
| OneBuyStatus| int | 是 |有效状态 0未开始，10进行中，11已结束 |
| OrganizationSysNo| int | 是 |平台编码 |
| DataRangeSysNo| int | 是 |店铺范围编码 |
| ProductGroupSysNo| int | 是 |款编码范围编码 |
| SortNo| int | 是 |排序 |

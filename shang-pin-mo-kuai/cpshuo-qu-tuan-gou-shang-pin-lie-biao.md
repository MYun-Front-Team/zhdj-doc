# CPS获取团购商品列表

CPS获取团购商品列表

_**【应用场景】**_

CPS获取团购商品列表
_**【接口地址】**_

http://ip:port/ProductQuery/ProductGroup/GetCPSGroupBuyList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 组织系统编码 |
| DataRangeSysNoList | int | 否 | 数据范围编码列表（店铺树） |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称\规格\标签） |
| IndustryClassSysNoList| array int | 否 | 行业类型分类系统编码（类别树） |
| TouristOrganizationSysNo | int | 是 | 游客组织系统编码（传0即为游客） |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

#### GroupBuy {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupBuySysNo| int | 是 | 系统编码 |
| ProductGroupName| string | 是 | 款名称 |
| IndustryClassSysNo| int | 是 | 行业类型分类系统编码（类别树） |
| IndustryClassName|string| 是 |行业类别名称|
| OnSaleStatus| int | 是 | 上下架 |
| ProductGroupClassName| int | 是 | 类别名称 |
| FileThumbnailUrlList| array string | 是 | 款缩略图 |
| CPSSysNo|int| 是 | CPS系统编码|
| CPSCode|string| 是 | CPSCode|
| Price|Price| 是 | 价格|
| OrganizationSysNo|int| 是 |组织系统编码|
| DataRangeSysNo|int| 是 |店铺数据范围|
| DataRangeName|string| 是 |店铺数据范围|
| SkuList|array Sku| 是 |店铺数据范围|
| CPSInOrderCount|int| 是 |评论数|
| CPSMaterialUrl|string| 是 |CPS落地页|
| CPSPromotionUrl|string| 是 |推广链接|





#### GroupBuySku {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SkuName| string | 是 | SKU名称 |
| Price|Price| 是 | 价格|
| FileThumbnailUrlList| array string | 是 | sku缩略图 |
| CPSCommission|decimal| 是 | CPS佣金|
| CPSCommissionRate|decimal| 是 | CPS佣金比率|
| SourceSkuCode| string | 是 | CPSSKU编码 |




#### Price {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SalePrice| int | 是 | 拼团价|
| MarketPrice| int | 是 | 单购价|
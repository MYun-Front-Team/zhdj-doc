# CPS获取商品详情

##### _【功能说明】_ {#【功能说明】}

CPS获取商品详情

_**【应用场景】**_

CPS获取商品详情

注：当DataRangeSysNo=0时，查询该商品所属组织的详情，否则则为该店铺的详情；

_**【接口地址】**_

http://ip:port/ProductQuery/ProductGroup/GetCPSProductGroupBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围结点（店铺树） |
| ProductGroupSysNo | int | 是 | 款系统编码 |
| TouristOrganizationSysNo | int | 是 | 游客组织系统编码（传0即为游客） |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

#### Group {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo| int | 是 | 款系统编码 |
| ProductGroupName| string | 是 | 款名称 |
| ProductGroupClassSysNo| int | 是 | 款类别编码 |
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
| CPSStartDate|datetime| 是 |推荐开始时间|
| CPSEndDate|datetime| 是 |推荐结束时间|
| CPSInOrderCount|int| 是 |评论数|
| IndustryClassSysNo|int| 是 |行业类别|
| IndustryClassName|string| 是 |行业类别名称|














#### Sku {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SkuSysNo| int | 是 | SKU系统编码 |
| SkuName| string | 是 | SKU名称 |
| Price|Price| 是 | 价格|
| FileThumbnailUrlList| array string | 是 | sku缩略图 |
| CPSCommission|decimal| 是 | CPS佣金|
| CPSCommissionRate|decimal| 是 | CPS佣金比率|
| SourceSkuCode| string | 是 | CPSSKU编码 |






#### Price {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SalePrice| int | 是 | 销售价|
| MarketPrice| int | 是 | 市场价|



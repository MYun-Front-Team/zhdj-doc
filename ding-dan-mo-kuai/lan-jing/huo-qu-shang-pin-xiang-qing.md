# 获取商品详情

获取商品详情

_**【应用场景】**_

获取商品详情

_**【接口地址】**_

http://ip:port/ProductQuery/LJProductGroup/GetLJProductGroupBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围结点（店铺树） |
| ProductGroupSysNo | int | 是 | 款系统编码 |




> #### _应答数据 _ {#应答数据-（巡河记录数组）}

#### Group {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo| int | 是 | 款系统编码 |
| ProductGroupName| string | 是 | 款名称 |
| ProductGroupClassSysNo| int | 是 | 款类别编码 |
| ProductGroupClassName| int | 是 | 类别名称 |
| FileThumbnailUrlList| array string | 是 | 款缩略图 |
| CPSSysNo|int| 是 | CPS系统编码|
| CPSCode|string| 是 | CPSCode|
| Price|Price| 是 | 价格|
| OrganizationSysNo|int| 是 |组织系统编码|
| DataRangeSysNo|int| 是 |店铺数据范围|
| ShopName|string| 是 |店铺名称|
| SkuList|array Sku| 是 |店铺数据范围|
| CPSInOrderCount|int| 是 |评论数|
| CPSMaterialUrl|string| 是 |CPS落地页|
| IndustryClassSysNo|int| 是 |行业类别|
| IndustryClassName|string| 是 |行业类别名称|
| ProductGroupMemo | string | 否 | 款备注 |
| FakeSaleCount|int| 是 |虚假销量|
| FileUrlList | array string | 否 | 买手头像图片列表 |
| IsWaitCode|int| 是 |是否待回填|
| LimitSubsidyMPStart | datetime | 否 | 限购魔力锁开始时间|
| LimitSubsidyMPEnd | datetime | 否 | 限购魔力锁结束时间|
| LimitSubsidyMPCount | int | 否 | 限购魔力锁最大份数|



#### Sku {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SkuSysNo| int | 是 | SKU系统编码 |
| SkuName| string | 是 | SKU名称 |
| Price|Price| 是 | 价格|
| FileThumbnailUrlList| array string | 是 | sku缩略图 |
| SourceSkuCode| string | 是 | CPSSKU编码 |



#### Price {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SalePrice| decimal| 是 | 券后价|
| MarketPrice| decimal| 是 | 市场价|
| RewardMP| decimal| 否 | 奖励魔力|
| CouponPrice| decimal | 否 | 优惠券金额 |
| ReturnPrice | decimal| 否 | 返还金额 |
| LJPrice | decimal\(18,2\) | 否 | 蓝晶价 |
| SubsidyMP | decimal | 否 | 补贴魔力 |









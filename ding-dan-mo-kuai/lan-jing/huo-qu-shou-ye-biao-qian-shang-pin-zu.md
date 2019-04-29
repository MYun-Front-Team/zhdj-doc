# 获取商品推荐列表

获取商品推荐列表

_**【应用场景】**_

获取商品推荐列表
_**【接口地址】**_

http://ip:port/ProductQuery/LJProductGroup/GetLJTagProductList



#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### _应答数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Tag | Tag | 是 |标签 |
| Groups | array[Group] | 是 |商品组 |


  #### Tag
| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TagSysNo | int | 是 | 系统编码 |
| TagName | string | 是 | 标签名称 |
| TagUrlList | array string | 否 | 标签URL列表 |
| PosterUrlList | array string | 否 | 海报URL列表 |
| IconColor | string | 否 | 标签底色 |
| SortNo | int | 是 | 排序 |


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



#### Sku {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SkuSysNo| int | 是 | SKU系统编码 |
| SkuName| string | 是 | SKU名称 |
| Price|Price| 是 | 价格|
| FileThumbnailUrlList| array string | 是 | sku缩略图 |
| SourceSkuCode| string | 是 | CPSSKU编码 |
| SkuInventory| SkuInventory | 是 | 库存信息|


#### SkuInventory

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PhysicalQuantity| int| 是 | 物理库存|
| AvailableQuantity| int| 是 | 可用库存|
| OrderLockQuantity| int| 是 | 锁定库存|




#### Price {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SalePrice| decimal| 是 | 券后价|
| MarketPrice| decimal| 是 | 市场价|
| RewardMP| decimal| 否 | 奖励魔力|





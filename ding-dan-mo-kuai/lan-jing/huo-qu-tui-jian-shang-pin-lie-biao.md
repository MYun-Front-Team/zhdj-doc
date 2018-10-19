# 获取商品推荐列表（福狸商城）

获取商品推荐列表（福狸商城）

_**【应用场景】**_

获取商品推荐列表（福狸商城）

_**【接口地址】**_

http://ip:port/ProductQuery/LJProductGroup/GetLJRecommendList



#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 所有者组织系统编码 |
| DataRangeSysNoList | array int | 否 | 数据范围系统编码（投放位置树） |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| RecommendStatusList | array int | 否 | 推荐状态：0未开始，1进行中，2已过期 |
| RecommendTypeList | array int | 否 | 推荐类型 |
| CategorySysNo | int | 否 | 推荐行业系统编码 |
| Limit| Limit| 是 | 显示限制|

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





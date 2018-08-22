# 获取商品推荐列表（福狸商城）

获取商品推荐列表（福狸商城）

_**【应用场景】**_

获取商品推荐列表（福狸商城）

_**【接口地址】**_

http://ip:port/ProductQuery/ProductGroup/GetFLRecommendList



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



#### _应答数据 _ {#应答数据-（巡河记录数组）}

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
| CPSInOrderCount|int| 是 |评论数|
| CPSMaterialUrl|string| 是 |CPS落地页|
| IndustryClassSysNo|int| 是 |行业类别|
| IndustryClassName|string| 是 |行业类别名称|
| FakeSaleCount|int| 是 |销售数|
| FakeInventoryCount|int| 是 |假库存数|
| SpecGroup | object | 否 | 规格组（说明见“获取规格模板列表”） |
| ProductGroupMemo | string | 否 | 款备注 |
| IsClearStocks | int | 否 | 是否是清货款：0否，1是 |
| CutCount|int| 是 |当前参与人数|
|CutPersons|array CutPerson| 是 |当前参与人|


#### CutPerson{#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FileUrlList| array string | 是 | 头像缩略图 |


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
| SpecValueList | array object | 否 | 规格值列表 |
| IsOneBuy| int | 否 | 是否是1元购 |
| OneBuyCount| int | 否 | 1元购分数 |
| IsGroupBuy| int | 否 | 是否是拼购 |
|CouponList| array Coupon | 否 |可使用优惠券 |

### Coupon

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CouponName| string| 是 | 优惠券名称|
| FullAmount| decimal| 是 | 优惠券使用金额条件|
| ReduceAmount| decimal| 是 | 优惠券金额|
| CPSMaterialUrl|string| 是 |CPS领取地址|


#### Price {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MinSalePrice| decimal| 是 | 砍到极限的销售价|
| MarketPrice| decimal| 是 | 市场价(严选价)|

#### Limit
| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowFileThumbnailUrlList | int | 否 | 是否显示缩略图列表（数量） |
| IsShowSkuList | int | 否 | 是否显示sku列表 |
| IsShowSpecGroup | int | 否 | 是否显示规格组（说明见“获取规格模板列表”） |
| IsShowSpecValueList | int | 否 | 是否显示规格值（当IsShowSkuList/IsShowSpecGroup=1时启用） |
| IsShowCouponList | int | 否 | 是否显示可用优惠券 |






# CPS获取商品详情

##### _【功能说明】_ {#【功能说明】}

CPS获取商品详情

_**【应用场景】**_

CPS获取商品详情

注：当DataRangeSysNo=0时，查询该商品所属组织的详情，否则则为该店铺的详情；

_**【接口地址】**_

http://ip:port/ProductQuery/ProductGroup/GetFLProductGroupBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围结点（店铺树） |
| ProductGroupSysNo | int | 是 | 款系统编码 |
| TouristOrganizationSysNo | int | 是 | 游客组织系统编码（传0即为游客） |
| Limit| Limit| 是 | 显示限制|





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
| CPSInOrderCount|int| 是 |评论数|
| CPSMaterialUrl|string| 是 |CPS落地页|
| IndustryClassSysNo|int| 是 |行业类别|
| IndustryClassName|string| 是 |行业类别名称|
| FakeSaleCount|int| 是 |销售数|
| FakeInventoryCount|int| 是 |假库存数|
| ProductGroupDetail|string| 是 |商品详情|
| SpecGroup | object | 否 | 规格组（说明见“获取规格模板列表”） |
| ProductGroupMemo | string | 否 | 款备注 |
| IsClearStocks | int | 否 | 是否是清货款：0否，1是 |






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




#### Price {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MinSalePrice| decimal| 是 | 砍到极限的销售价|
| MarketPrice| decimal| 是 | 市场价(严选价)|
| MaxHelpPrice| decimal| 是 | 最大帮砍奖励|
| MinHelpPrice| decimal| 是 | 最小帮砍奖励|
| MinFansReward| decimal| 是 | 最小粉丝购物奖励|
| MaxFansReward| decimal| 是 | 最大粉丝购物奖励|


#### Limit
| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowFileThumbnailUrlList | int | 否 | 是否显示缩略图列表（数量） |
| IsShowSkuList | int | 否 | 是否显示sku列表 |
| IsShowSpecGroup | int | 否 | 是否显示规格组（说明见“获取规格模板列表”） |
| IsShowSpecValueList | int | 否 | 是否显示规格值（当IsShowSkuList/IsShowSpecGroup=1时启用） |





































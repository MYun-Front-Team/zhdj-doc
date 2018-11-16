#获取我的砍价商品详情

获取我的砍价商品详情

_**【应用场景】**_

获取我的砍价商品详情

_**【接口地址】**_

http://ip:port/ShopQuery/CutPirce/GetMyFLCutPirceBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CutPirceSysNo| int | 是 | 砍价系统编码 |




> #### _应答数据 _ {#应答数据-（巡河记录数组）}

#### CutPirce {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CutPirceSysNo| int | 是 | 砍价系统编码 |
| PersonSysNo| int | 否 | 发起人员系统编码 |
| ProductGroupSysNo| int | 是 | 款系统编码 |
| ProductGroupName| string | 是 | 款名称 |
| ProductGroupClassSysNo| int | 是 | 款类别编码 |
| OnSaleStatus| int | 是 | 上下架 |
| ProductGroupClassName| int | 是 | 类别名称 |
| FileThumbnailUrlList| array string | 是 | 款缩略图 |
| CPSSysNo|int| 是 | CPS系统编码|
| CPSCode|string| 是 | CPSCode|
| OrganizationSysNo|int| 是 |组织系统编码|
| DataRangeSysNo|int| 是 |店铺数据范围| 
| DataRangeName|string| 是 |店铺数据范围|
| CPSInOrderCount|int| 是 |评论数|
| CPSMaterialUrl|string| 是 |CPS落地页|
| IndustryClassSysNo|int| 是 |行业类别|
| IndustryClassName|string| 是 |行业类别名称|
| RemaindSecond| int| 是 | 砍价剩余时间秒|
| Sku | Sku  | 是 | SKU系统编码 |
| NowPirce| decimal | 是 | 当前砍至价格|
| CutPirceStatus| int | 是 | 砍价状态（1进行中，11取消，9完成，10最终确认） |
| ProductGroupDetail|string| 是 |商品详情|
| FinishRemaindSecond| int| 是 | 强制完结剩余时间秒|
| FakeSaleCount|int| 是 |销售数|
| FakeInventoryCount|int| 是 |假库存数|
| ProductGroupMemo | string | 否 | 款备注 |
| BrandList | array object | 否 | 品牌列表（说明见通用） |
| CutPirceType|int| 是 |砍价类型（1普通砍价 2自营一元购）|
| MinCPSPirce| decimal| 是 | 必砍价 |
| ReduceCount|int| 是 |预估刀数|
| HaveReduceCount|int| 是 |已砍刀数|
| OrderSysNo|int| 是 |订单编码|
| SourceOrderCode|string| 是 |三方订单号|
| CancelStatus | int | 是 | 取消状态：0正常，1取消中，10已消，11取消失败 |

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
| MinSalePrice| decimal| 是 | 砍到极限的销售价|
| MarketPrice| decimal| 是 | 市场价(严选价)|
| MaxHelpPrice| decimal| 是 | 最大帮砍奖励|
| MinHelpPrice| decimal| 是 | 最小帮砍奖励|
| MinFansReward| decimal| 是 | 最小粉丝购物奖励|
| MaxFansReward| decimal| 是 | 最大粉丝购物奖励|



# 获取商品列表

获取商品列表

_**【应用场景】**_

获取商品列表

_**【接口地址】**_

http://ip:port/ProductQuery/LJProductGroup/GetLJProductGroupPriceByCode

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SourceProductGroupCodeList |array[string] | 否 | 组织系统编码 |



> #### _应答数据 _ {#应答数据-（巡河记录数组）}

#### Group {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SourceProductGroupCode| string | 是 | 三方款编码 |
| Price|Price| 是 | 价格|


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


# 获取蓝晶/魔力

获取蓝晶/魔力

_**【应用场景】**_

获取蓝晶/魔力

_**【接口地址】**_

http://ip:port/PointQuery/LJPoint/GetLJPoint



#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PointsType| int| 是 | 积分类型 |





#### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Total| Total| 是 | 积分汇总 |
| Items| array[Item]| 是 | 积分明细 |



#### Total

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PointsValue| decimal| 是 | 当前积分 |
| AvaPointsValue| decimal| 是 | 可用积分 |
| FroPointsValue| decimal| 是 | 冻结积分 |
| HisPointsValue| decimal| 是 | 历史积分 |
| UncPointsValue| decimal| 是 | 不可转换积分 |





#### Item

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








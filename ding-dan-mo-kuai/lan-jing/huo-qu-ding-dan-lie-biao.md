#获取订单列表

##### _【功能说明】_ {#【功能说明】}

获取订单列表

_**【应用场景】**_

获取订单列表

_**【接口地址】**_

http://ip:port/OrderQuery/LJOrder/GetLJOrderList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| KeyWord| string| 否 | 关键字 |
| OrganizationFromSysNo | int | 否 | 卖家组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围树编码（店铺树） |
| OrganizationToSysNo | int |否 | 买家组织系统编码 |
| PersonSysNo | int | 否 | 买家人员系统编码 |
| OrderStatus| int | 否 | 订单状态（1待填订单号，2等待奖励，10已完成，11已关闭，12订单有误） |
| SettlementStatusList|array[int] | 否 |结算状态（10已结算，0待结算）|
| SourceOrderCode | string | 否 | 订单来源订单号 |
| StartFillSourceOrderCodeTime| datetime| 是 | 开始填三方订单号时间|
| EndFillSourceOrderCodeTime| datetime| 是 | 结束填三方订单号时间|
| OrderStartTime | string | 否 | 开始时间（订单创建时间） |
| OrderEndTime | string | 否 | 结束时间（订单创建时间） |
| ProductGroupName| string| 否 | 商品名称 |
| CellPhoneNo| string| 否 | 手机号 |
| StartRewardMP| decimal | 否 | 开始奖励魔力|
| EndRewardMP| decimal | 否 | 终止奖励魔力|
| CPSCode | string | 否 | 三方来源编号 |
| NoCPSCode | string | 否 | 除三方来源编号 |
| TagName | string | 否  | 标签名称 |
| TagType| int | 否 | 标签类型 |




> #### 返回数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Total| Total| 否 |统计信息 |
| Details| array[Detail]| 否 |订单列表信息 |

#### Total

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RewardMP| decimal| 否 | 总奖励魔力|
| WaitCodeCount| int| 否 | 待填订单号数量|
| WaitRewardCount| int| 否 | 等待奖励数量|
| ErrorCount| int| 否 | 订单有误数量|


#### Detail

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 否 | 买家人员系统编码 |
| OrganizationFromSysNo | int | 是 | 卖家组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树编码（店铺树） |
| OrganizationToSysNo | int | 是 | 买家组织系统编码 |
| PersonSysNo | int | 是 | 买家人员系统编码 |
| OrderStatus| int | 是 | 订单状态（1待填订单号，2等待奖励，10已完成，11已关闭，12订单有误） |
| WaitCodeSecond| int| 否 | 待填订单号秒数|
| SourceOrderCode| string| 是 | 三方订单号|
| DetailItems| array[DetailItem]| 是 | 三方订单号|
| PersonName | string| 是 | 买家人员昵称 |
| CellPhoneNo| string| 是 | 买家人员手机 |
| FillSourceOrderCodeTime| datetime| 是 | 填三方订单号时间|
| CreateTime| datetime| 是 | 创建时间 |
| TotalPrice| decimal | 否 | 总价|
| TotalRewardMP| decimal | 否 | 总奖励魔力|
| TotalRewardAmount| decimal | 否 | 总奖励金额|
|CommentStatus|int | 是 | 评价状态（0未评价，10已经评价）|
| SettlementStatus| int | 是 | 结算状态（10已结算，0待结算） |
| AuditStatus| int | 是 | 审核状态（0待审核，10审核通过，11审核不通过） |
| TagList | array object | 否 | 标签列表（说明见通用） |
| CPSCode | string | 否 | 三方来源编号 |

####Tag

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TagSysNo | int | 是 | 系统编码 |
| TagName | string | 是 | 标签名称 |
| IconColor | string | 否 | 标签底色 |



#### DetailItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo| int | 否 | 款系统编码 |
| SkuSysNo| int | 否 | SKU系统编码 |
| Quantity| int | 否 | 数量 |
| UnitPrice| decimal | 否 | 单价|
| RealPrice| decimal | 否 | 总价|
| Const| decimal | 否 | 成本价|
| RewardMP| decimal | 否 | 奖励魔力|
| ProductGroupName| string| 否 | 商品名称 |
| CPSSysNo| int | 是 | CPS系统编码 |
| CPSCode| string| 是 | CPS编号 |
| FileThumbnailUrlList| array string | 是 | 款缩略图 |
| CouponPrice| decimal\(18,2\) | 否 | 优惠券金额 |




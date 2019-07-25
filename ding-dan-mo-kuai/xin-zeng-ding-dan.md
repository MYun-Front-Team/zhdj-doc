# 新增订单 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增订单

_**【应用场景】**_

新增订单

注：1、通过组织间关系获取商品实时价格；

2、新增商品后把商品当前的冗余信息保存到“订单商品冗余表”；

3、限制库存的SKU需要判断库存是否充足；（订单锁）

4、PlatformAuditStatus=0则订单需要审核，PlatformAuditStatus=10则订单自动已审核，可直接支付。

5、桃子乐采，订单类型23001
支付方式：13拍宝付 4线下汇款14信用支付

_**【接口地址】**_

[http://ip:port/OrderAction/](http://ip:port/HMAction/River/AddRiver)Order[/A](http://ip:port/HMAction/River/AddRiver)ddOrder

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationFromSysNo | int | 是 | 卖家组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树编码（店铺树） |
| OrganizationToSysNo | int | 是 | 买家组织系统编码 |
| PersonSysNo | int | 否 | 买家人员系统编码 |
| OrderType | int | 是 | 订单类型（枚举） |
| OrderClassSysNo | int | 否 | 订单分类（枚举） |
| OrderSource | int | 是 | 订单来源（枚举） |
| SourceOrderCode | string | 否 | 订单来源订单号 |
| PaymentType | int | 否 | 支付方式（枚举） |
| TrackingCompanySysNo | int | 否 | 期望快递公司系统编码(或配送方式） |
| ReceiverName | string | 是 | 收货人 |
| ReceiverPhone | string | 是 | 收货电话 |
| ReceiverAddress | string | 是 | 收货地址 |
| PCDCode | string | 否 | 省市区 代码 |
| PCDDescription | string | 否 | 省市区 名称 |
| IsNeedBill | int | 否 | 是否需要发票 |
| BillName | string | 否 | 发票抬头 |
| BillType | int | 否 | 发票类型：1企业，2机构，3个人 |
| BillCode| string | 否 | 税号 |
| OrderRemark | string | 否 | 订单买家备注 |
| AddOrderItemList | array object | 是 | 订单商品列表 |
| AddOrderAmountList | array object | 否 | 订单优惠列表 |
| PrivacyPropertys | array object | 否 | 隐私属性列表 |
| CouponCodes | array string | 否 | 订单优惠券码 |
| IsDoortodoor|int | 是 | 是否上门服务|
| CPSSysNo| int | 是 | CPS系统编码 |
| InvitationCode| string | 否 | 邀请码 |
| RelativeOrderSysNo | int | 否 | 来源订单 |
 




> #### AddOrderItem订单商品列表 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo | int | 是 | 款号系统编码 |
| SkuSysNo | int | 是 | SKU系统编码 |
| CustomizedSpecValue | string | 否 | 可定制规格值 |
| Quantity | int | 是 | 购买数量 |
| RealPrice | decimal\(18,2\) | 否 | 单价 |
| Remark | string | 否 | 备注|


> #### AddOrderAmount订单优惠金额列表 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AmountType | int | 是 | 类型：7客服优惠金额，8运费优惠金额 |
| Amount | decimal（18，2） | 是 | 优惠金额 |
| Remark | string | 否 | 备注 |

> #### 应答_数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 订单系统编码 |




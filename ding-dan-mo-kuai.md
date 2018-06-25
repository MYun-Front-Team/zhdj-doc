# 订单模块-字段说明 {#新增河流}

> #### Order基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 系统编码 |
| OrganizationFromSysNo | int | 是 | 卖家组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树编码（店铺树） |
| OrganizationToSysNo | int | 是 | 买家组织系统编码 |
| PersonSysNo | int | 是 | 买家人员系统编码 |
| OrderType | int | 是 | 订单类型：23001普通订单，23002预采购订单（点东东），23003采购单（翰想汇）,23004积分单，23005 CPS单，23006砍价单 |
| OrderClassSysNo | int | 是 | 订单分类：0正常订单，1合单订单，2拆单订单 |
| RelativeOrderSysNo | int | 否 | 合单，存储 To 关系；拆单，存储 From 关系 |
| OrderCode | string | 是 | 订单号 |
| OrderSource | int | 是 | 订单来源: 1后台,2官网,3IOS,4-安卓,5-HTML5,6第三方订单 |
| PaymentType | int | 是 | 支付方式：0余额，1支付宝，2微信，3银联，4线下，5刷卡,6积分，99混合 |
| SourceOrderCode | string | 否 | 订单来源订单号 |
| AuditStatus | int | 是 | 审核状态：0待审核，10已审核 |
| PaymentStatus | int | 是 | 支付状态：0未支付，1部分支付，10已支付 |
| DeliveryStatus | int | 是 | 发货状态：0未发货，1部分发货，10已发货 |
| ReceiveStatus | int | 是 | 收货状态：0未收货，1部分收货，10已收货，11拒收 |
| CancelStatus | int | 是 | 取消状态：0正常，1取消中，10已消，11取消失败 |
| FinishStatus | int | 是 | 完结状态，0未完结，10已完结 |
| SettlementStatus | int | 是 | 结算状态：0未结算，1部分结算，10已结算 |
| TrackingCompanySysNo | int | 否 | 期望快递公司系统编码 |
| ReceiverName | string | 是 | 收货人 |
| ReceiverPhone | string | 是 | 收货电话 |
| ReceiverAddress | string | 是 | 收货地址 |
| PCDCode | string | 是 | 省市区 代码 |
| PCDDescription | string | 是 | 省市区 名称 |
| IsNeedBill | int | 否 | 是否需要发票 |
| BillName | string | 否 | 发票抬头 |
| BillType | int | 否 | 发票类型：1企业，2机构，3个人 |
| BillCode| string | 否 | 税号 |
| OrderRemark | string | 否 | 订单买家备注 |
| DeliveryRemark | string | 否 | 订单卖家备注 |
| OrderItemList | array object | 否 | 订单商品列表 |
| OrderAmountList | array object | 否 | 订单金额列表 |
| OrderPaymentList | array object | 否 | 订单支付列表 |
| OrderCouponList | array object | 否 | 订单优惠列表 |
| ~~OrderLogList~~ | ~~array object~~ | ~~否~~ | ~~订单日志列表（通用日志）~~ |
| OrderDeliveryList | array object | 否 | 订单发货列表 |
| FromOrganization | object | 否 | 卖家组织实体（简版） |
| FromShop | object | 否 | 卖家店铺实体（简版） |
| ToOrganization | object | 否 | 买家组织实体（简版） |
| ToPerson | object | 否 | 买家人员实体（简版） |
| ToCustomer | object | 否 | 买家客户实体（简版） |
| FromSeller | object | 否 | 商家实体（简版） |
| PrivacyPropertys | array object | 否 | 隐私属性列表 |
| CouponCodeUseStatus | int | 是 | 服务订单使用情况：0未使用，1部分使用，10已使用 |
| IfOverdueStauts | int | 是 | 服务订单是否失效（0未失效1已失效2部分失效） |
|CommentStatus|int | 是 | 评价状态（0未评价，10已经评价）|
|IsDoortodoor|int | 是 | 是否上门服务|
| CPSSysNo| int | 是 | CPS系统编码 |
| CPSCode| string| 是 | CPS名称 JD京东，YX严选 |





#### OrderAmount说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderAmountSysNo | int | 是 | 订单金额系统编码 |
| AmountType | int | 是 | 业务逻辑自定义金额类型:0商品原始金额，1运费，2预收款，3活动优惠金额，4优惠券优惠金额，5积分抵扣金额，6实际支付总金额，7客服优惠金额，8运费优惠金额，9原始订单总金额，10当前商品总金额, 11商品佣金,12CPS佣金 |
| Amount | decimal（18，2） | 是 | 金额 |
| Remark | string | 否 | 备注 |

#### OrderPayment说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderPaymentSysNo | int | 是 | 订单支付系统编码 |
| PaymentType | int | 是 | 支付方式（枚举） |
| TradeNo | string | 否 | 交易号 |
| TotalFee | decimal（18，2） | 是 | 交易金额 |
| PayTime | string | 是 | 支付时间 |
| BuyerID | string | 否 | 买家帐户 |
| SellerID | string | 否 | 卖家帐户 |
| Remark | string | 否 | 备注 |

#### OrderCoupon说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderCouponSysNo | int | 是 | 订单支付系统编码 |
| CouponType | int | 是 | 优惠券类型：0自定义，1免邮，2邮费减免，3满减 |
| CouponSysNo | int | 是 | 优惠券编码 |
| CouponCode | string | 否 | 优惠代码 |
| CouponAmount | decimal（18，2） | 是 | 优惠金额\(减免金额\) |
| Remark | string | 否 | 备注 |

> #### OrderDelivery说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderDeliverySysNo | int | 是 | 订单发货单系统编码 |
| DeliveryStatus | int | 是 | 发货状态：0未发，10已发，11已取消 |
| DeliveryDate | string | 否 | 发货时间 |
| TrackingNo | string | 否 | 快递单号 |
| TrackingCompany | object | 否 | 快递公司实体（见通用） |

> #### Order统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderTimeList | array object | 否 | 订单操作时间列表 |
| IsServiceOrder | int | 否 | 是否服务订单：0否，1是 |
| AutoReceiveLeftMinutes| int | 否 |自动签收时间 |
| AutoCancelLeftMinutes| int | 否 | 自动取消时间 |






> #### OrderTime {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderAuditTime | string | 否 | 订单审核时间 |
| OrderPayTime | string | 否 | 订单支付时间 |
| OrderDeliveryTime | string | 否 | 订单发货时间 |
| OrderReceiveTime | string | 否 | 订单收货时间 |
| OrderFinishTime | string | 否 | 订单完结时间 |
| OrderSettlementTime | string | 否 | 订单结算时间 |
| OrderCancelTime | string | 否 | 订单取消时间 |

> #### OrderItem基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderItemSysNo | int | 是 | 系统编码 |
| ProductGroupSysNo | int | 是 | 款号系统编码 |
| SkuSysNo | int | 是 | SKU系统编码 |
| Sku | object | 否 | sku实体（见商品） |
| CustomizedSpecValue | string | 否 | 可定制规格值 |
| UnitPrice | decimal（18，2） | 是 | 单价 |
| RealPrice | decimal（18，2） | 是 | 实际价格 |
| OriginalQuantity | int | 是 | 原始购买数量 |
| Quantity | int | 是 | 最终购买数量 |
| OrderItemLockInventory | object | 否 | 订单商品锁库（见仓储） |
| DeliveriedQuantity | int | 否 | 已发货数量 |
| DeliveryItemStatus | int | 否 | 0未发，1部分发，10已发，11取消 |
| PointPrice| int | 是 | 积分单价 | 
| Remark | string | 否 | 备注|


> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderType | int | 是 | 订单类型（枚举） |
| OrganizationFromSysNo | int | 否 | 卖家组织系统编码 |
| DataRangeSysNoList | array int | 否 | 数据范围编码列表（店铺树） |
| OrganizationToSysNo | int | 否 | 买家组织系统编码 |
| PersonSysNoList | array int | 否 | 买家人员系统编码 |
| KeyWord | string | 否 | 关键字搜索（订单号/收货人/收货手机） |
| AuditStatusList | array int | 否 | 审核状态 |
| PaymentStatusList | array int | 否 | 支付状态 |
| DeliveryStatusList | array int | 否 | 发货状态 |
| ReceiveStatusList | array int | 否 | 收货状态 |
| CancelStatusList | array int | 否 | 取消状态 |
| FinishStatusList | array int | 否 | 完结状态 |
| SettlementStatusList | array int | 否 | 结算状态 |
| PaymentTypeList | array int | 否 | 支付方式 |
| OrderStartTime | string | 否 | 开始时间（订单创建时间） |
| OrderEndTime | string | 否 | 结束时间（订单创建时间） |
| CardNo | string | 否 | 会员卡号 |
| ShopName | string | 否 | 店铺名称 |
| CouponCodeUseStatusList | array int | 否 | 服务订单使用情况：0未使用，1部分使用，10已使用 |
| IfOverdueStautsList | array int | 是 | 服务订单是否失效（0未失效1已失效2部分失效） |
| IsServiceOrder | int | 否 | 是否是服务订单 |
|CommentStatusList| array int | 是 | 评价状态（0未评价，10已经评价）|
| CPSCode| string| 是 | CPS名称 JD京东，YX严选 |






> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderLimit | object | 否 | 订单限制条件 |
| ProductLimit | object | 否 | 商品限制条件（见商品说明） |

#### OrderLimit说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowOrderAmountList | int | 否 | 是否显示订单金额列表 |
| IsShowOrderPaymentList | int | 否 | 是否显示订单支付列表 |
| IsShowOrderCouponList | int | 否 | 是否显示订单优惠列表 |
| ~~IsShowOrderLogList~~ | ~~int~~ | ~~否~~ | ~~是否显示订单日志列表~~ |
| IsShowOrderItemList | int | 否 | 是否显示订单商品列表 |
| IsShowOrderItemSku | int | 否 | 是否显示订单商品SKU（只有IsShowOrderItemList=1才有效） |
| IsShowOrderDeliveryList | int | 否 | 是否显示订单发货单列表 |
|  |  |  |  |
| IsShowFromOrganization | int | 否 | 是否显示卖家组织 |
| IsShowFromShop | int | 否 | 是否显示卖家店铺 |
| IsShowToOrganization | int | 否 | 是否显示买家组织 |
| IsShowToPerson | int | 否 | 是否显示买家人员 |
| IsShowOrderTimeList | int | 否 | 是否显示订单时间列表 |
| IsShowDeliveriedQuantity | int | 否 | 是否显示已发数量 |
| IsShowToCustomer | int | 否 | 是否显示买家客户 |
| IsShowFromSeller | int | 否 | 是否显示商家 |
| IsShowPrivacyPropertys | int | 否 | 是否显示隐私属性 |
| IsShowIsServiceOrder | int | 否 | 是否显示是否服务订单 |
| IsShowLeftMinutes | int | 否 | 是否显示剩余操作时间 |



#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |
| 2300101 | 订单模块 | 普通订单 |  | 新增页 |
| 2300102 |  | 普通订单 |  | 修改页 |
| 2300103 |  | 普通订单 |  | 详情页 |
| 2300104 |  | 普通订单 |  | 列表页 |




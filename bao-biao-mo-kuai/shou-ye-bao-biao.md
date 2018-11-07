# 首页报表 {#获取河长巡河记录}

#### 页面编号枚举说明 {#请求数据}

| 页编码 | 模块说明 | 页面说明 |
| :--- | :--- | :--- |
| 100 | 首页报表 | 智慧市场-APP商家首页 |
| 101 | 首页报表 | 点东东-平台APP |
| 102 | 首页报表 | 翰想汇-微信端个人中心首页 |
| 103 | 首页报表 | 智慧园区-app个人中心首页 |
| 104 | 首页报表 | 招聘首页-app个人中心首页 |
| 105 | 首页报表 | 蓝晶社-app个人中心首页 |








> #### _请求数据（PageRequestData）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围树编码（店铺树） |

> #### _应答数据 （PageResponseBase）【100】_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OnSaleProductCount | int | 是 | 在售商品总数 |
| SaleTotalAmountInToday | decimal\(18,2\) | 是 | 今日销售总额 |
| BalanceAmount | decimal\(18,2\) | 是 | 钱包余额 |
| UnDoOrderTotalNum | int | 是 | 待处理订单总数 |
| UnDoOrderTotalNum | int | 是 | 待处理订单总数 |
| PlatformOnSaleProductCount | int | 是 | 平台可订货|
| PurchaseOrderFinish | int | 是 | 商品已采购订货单|
| PurchaseOrderNotFinish | int | 是 | 商品未采购订货单|
| PurchaseOrderNotPaid| int | 是 | 商品未支付订货单|
| PlatformPurchaseOrderNotFinish | int | 是 | 平台未采购数量|
| FrozenPurchaseOrderTotalAmount| decimal | 是 | 冻结钱包采购总金额|


#### 注：上述参数全部以【key，value】键值对形势返回； {#应答数据-（巡河记录数组）}

#### _应答数据 （PageResponseBase）【101】_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SellerCount | int | 是 | 商家总数 |
| AuditSellerCount | int | 是 | 待审核商家总数 |
| ProductCount | int | 是 | 商品总数 |
| OnSaleProductCount | int | 是 | 已上架商品总数 |
| MessageCount | int | 是 | 消息总数 |
| UnReadedMessageCount | int | 是 | 未读消息总数 |

#### _应答数据 （PageResponseBase）【102】_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FavoriteProductCount | int | 是 | 收藏商品总数 |
| FavoriteShopCount | int | 是 | 收藏店铺总数 |
| FavoriteFootCount | int | 是 | 足迹总数（暂为0） |
| OrderPayingCount | int | 是 | 待付款订单总数 |
| OrderSendingCount | int | 是 | 待发货订单总数 |
| OrderReceivingCount | int | 是 | 待收货订单总数（邮寄类订单） |
| OrderUsingCount | int | 是 | 待使用订单总数（到店消费订单） |
| OrderCommentCount | int | 是 | 待评论订单总数 |

#### _应答数据 （PageResponseBase）【103】_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SellerInfos | array SellerInfo | 是 | 企业信息 |
| ParkProjectInfos | array ParkProjectInfo | 是 | 招商管理 |
| WaitPaySellerCount | int | 是 | 待缴费企业 |
| WaitPaySellerAmount | decimal | 是 | 待缴费金额 |



#### SellerInfo

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SellerClassSysNo | int | 是 | 企业类别 |
| Count| int | 是 |数量 |

#### ParkProjectInfo

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProjectStatus | int | 否 |项目状态（0潜在，1洽谈，2入住，3长期） |
| Count| int | 是 |数量 |

> #### _应答数据 （PageResponseBase）【104】_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AuditStatusInfos| array[AuditStatusInfo] | 是 | 审核状态信息|
| RecruitPersonStatusInfos| array[RecruitPersonStatusInfo]| 否 |抢班状态  |

#### AuditStatusInfo

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AuditStatus| int| 是 | 岗位审核状态（0待审核 10已经审核 11审核不通过）|
| Count| int| 是 | 数量|

###RecruitPersonStatusInfo

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitPersonStatus| int| 是 |状态：0圈中，1已抢，2忽略，10抢中，11已失效，12拒绝，20已上班，21放鸽子|
| Count| int| 是 | 数量|


#### _应答数据 （PageResponseBase）【105】_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MPPoints| decimal | 否 | 魔力|
| LANPoints| decimal | 否 | 蓝晶|
| Commission| decimal | 否 | 效果预估佣金 |
| FinishCommission| decimal（18，10） | 是 | 结算效果预估 |
| AvailableAmount | decimal（18，2） | 是 | 钱包可用余额|
| AvailableReceiveCashAmount | decimal（18，2） | 是 | 钱包可提现金额|














# 钱包模块-字段说明 {#新增河流}

> #### 基础字段（Wallet） {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WalletSysNo | int | 是 | 钱包系统编码 |
| BalanceAmount | decimal（18，2） | 是 | 钱包余额（实际存在） |
| FrozenAmount | decimal（18，2） | 是 | 冻结余额1（如待提现冻结） |
| AvailableAmount | decimal（18，2） | 是 | 可用余额=钱包余额-冻结余额1 |
| TotalAmount | decimal（18，2） | 是 | 钱包总额=钱包余额+冻结余额2 |
|  |  |  |  |
| FrozenOrderAmount | decimal（18，2） | 是 | 冻结余额2（如未结算订单冻结） |
| InComeTotalAmount | decimal（18，2） | 是 | 收入总金额（订单+佣金等） |
| ReceiveCashTotalAmount | decimal（18，2） | 是 | 提现总金额（已提现+待提现） |
| AvailableReceiveCashAmount | decimal（18，2） | 是 | 可提现金额=收入总金额-提现总金额 |
|  |  |  |  |
| BondFee | decimal（18，2） | 否 | 保证金 |
| MemberShipFee | decimal（18，2） | 否 | 会员费 |
| MemberShipEndDate | string | 否 | 会员费到期时间 |
| MemberShipStatus | string | 否 | 当前会员费有效状态10有效，0无效 |
|  |  |  |  |
| FrozenCommissionAmount | decimal（18，2） | 否 | 冻结佣金金额（来源分润） |
| CommissionTotalAmount | decimal（18，2） | 否 | 佣金总金额（来源分润） |
| AgentFee | decimal（18，2） | 否 | 代理费 |
| AgentFeeEndDate | decimal（18，2） | 否 | 代理费到期时间 |
| AgentFeeStatus | int | 否 | 当前代理费有效状态10有效，0无效 |
| AvailablePoint | int | 是 | 可支付积分余额|
| WxPurchaseOrderTotalAmount| decimal | 是 | 微信采购总金额|
| AlPurchaseOrderTotalAmount| decimal | 是 | 支付宝采购总金额|
| WalletPurchaseOrderTotalAmount| decimal | 是 | 钱包采购总金额|
| FrozenPurchaseOrderTotalAmount| decimal | 是 | 冻结钱包采购总金额|











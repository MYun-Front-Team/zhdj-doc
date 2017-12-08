# 钱包模块-字段说明 {#新增河流}

> #### 基础字段（Wallet） {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WalletSysNo | int | 是 | 钱包系统编码 |
| BalanceAmount | decimal（18，10） | 是 | 钱包余额（实际存在） |
| FrozenAmount | decimal（18，10） | 是 | 冻结余额（如提现冻结） |
| AvailableAmount | decimal（18，10） | 是 | 可用余额=钱包余额-冻结余额 |




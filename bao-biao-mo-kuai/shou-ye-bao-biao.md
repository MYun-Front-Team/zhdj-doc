# 首页报表 {#获取河长巡河记录}

#### 页面编号枚举说明 {#请求数据}

| 页编码 | 模块说明 | 页面说明 |
| :--- | :--- | :--- |
| 100 | 首页报表 | 智慧市场-APP商家首页 |
| 101 | 首页报表 | 点东东-平台APP |

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




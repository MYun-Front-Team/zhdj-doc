# 订单报表 {#获取河长巡河记录}

#### 页面编号枚举说明 {#请求数据}

| 页编码 | 模块说明 | 页面说明 |
| :--- | :--- | :--- |
| 23000100 | 订单报表 | 按客户维度 |
| 23000101 | 订单报表 | 按订单维度 |
| 23000102 | 订单报表 | 按日期维度 |
| 23000103 | 订单报表 | 按款号维度 |
| 23000104 | 订单报表 | 按商家统计（平台查看） |

> #### _请求数据（PageRequestData）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationFromSysNo | int | 是 | 卖家组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围树编码（店铺树） |
| PersonFromSysNo | int | 否 | 卖家人员系统编码 |
| OrganizationToSysNo | int | 否 | 买家组织系统编码 |
| PersonSysNo | int | 否 | 买家人员系统编码 |
| OrderStartTime | string | 否 | 订单开始时间 |
| OrderEndTime | string | 否 | 订单结束时间 |

> #### _应答数据 （PageResponseBase）【23000100】_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationToSysNo | int | 是 | 买家组织系统编码 |
| CustomerSysNo | int | 是 | 客户系统编码 |
| CustomerName | string | 是 | 客户名称 |
| OrderTotalNum | int | 是 | 订单总数 |
| OrderTotalAmount | decimal\(18,2\) | 是 | 订单总金额 |

#### _应答数据 （PageResponseBase）【23000101】_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 订单编码 |
| OrderCode | string | 是 | 订单号 |
| OrganizationToSysNo | int | 是 | 买家组织系统编码 |
| CustomerSysNo | int | 是 | 客户系统编码 |
| CustomerName | string | 是 | 客户名称 |
| OrderItemNum | int | 是 | 订单商品总数 |
| OrderAmount | decimal\(18,2\) | 是 | 订单金额 |

#### _应答数据 （PageResponseBase）【23000102】_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderDate | string | 是 | 日期（yyyy-MM-dd） |
| OrderTotalNum | int | 是 | 订单总数 |
| OrderTotalAmount | decimal\(18,2\) | 是 | 订单总金额 |

#### _应答数据 （PageResponseBase）【23000103】_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo | int | 是 | 款系统编码 |
| ProductGroupCode | string | 是 | 款号 |
| OrderTotalNum | int | 是 | 订单总数 |
| OrderTotalAmount | decimal\(18,2\) | 是 | 订单总金额 |

#### _应答数据 （PageResponseBase）【23000104】_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SellerSysNo | int | 是 | 商家系统编码 |
| SellerName | string | 是 | 商家名称 |
| OrderTotalNum | int | 是 | 订单总数 |
| OrderTotalAmount | decimal\(18,2\) | 是 | 订单总金额 |




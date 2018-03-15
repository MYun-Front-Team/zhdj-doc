# 工单报表 {#获取河长巡河记录}

#### 页面编号枚举说明 {#请求数据}

| 页编码 | 模块说明 | 页面说明 |
| :--- | :--- | :--- |
| 24000100 | 资金报表 | 按区域维度 |

> #### 请求数据（PageRequestData）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WorkType| int | 是 | 工单类型 |
> #### 应答数据 （PageResponseBase）【24000100】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PaymentStatisticsList | array object | 是 | 支付统计 |
| OrderPaymentList | array object | 是 | 支付记录列表 |

#### PageResponseStatistic【24000100】 说明

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PaymentType | int | 是 | 支付方式 |
| TotalAmount | decimal\(18,2\) | 是 | 支付总金额 |
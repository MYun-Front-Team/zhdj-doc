# 审核退货

##### _【功能说明】_ {#【功能说明】}

审核退货

_**【应用场景】**_

审核退货
1（仅退款的退货单调用不能调用此接口）
2（退货退款的退货单，卖家同意退货时调用）


_**【接口地址】**_

http://ip:port/OrderAction/RMA/GoodBackOrderRMA

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RMASysNo | int | 是 | 退货单系统编码 |
| AuditRemark | string | 否 | 审核备注 |
| AuditStatus | int | 是 | 审核状态：10同意退货，11不同意退货 |
| RMAReceiverAddress| string| 是 | 退货地址 |
| RMAReceiverName| string| 是 | 退货收货人 |
| RMAReceiverPhone| string| 是 | 退货收货人电话|


> #### 应答_数据_ {#请求数据}



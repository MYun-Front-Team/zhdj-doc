# 申请退货/退款



##### _【功能说明】_ {#【功能说明】}

申请退货/退款

_**【应用场景】**_

申请退货/退款




_**【接口地址】**_

http://ip:port/OrderAction/RMA/AddOrderRMA

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderItemSysNo | int | 是 | 订单明细系统编码 |
| RMAReason| string| 是 | 退货理由 |
| Remark | string | 否 | 退货备注 |
| FilePathList | array string | 否 | 图片列表 |
| RMAAmount| decimal| 是 | 退款金额 |
| RMACount| int | 是 | 数量 |











> #### 应答_数据_ {#请求数据}




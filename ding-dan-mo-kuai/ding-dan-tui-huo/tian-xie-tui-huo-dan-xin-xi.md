# 申请退货

##### _【功能说明】_ {#【功能说明】}

申请退货

_**【应用场景】**_

申请退货


_**【接口地址】**_

http://ip:port/OrderAction/RMA/AddOrderRMA

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RMASysNo | int | 是 | 退货单系统编码 |
| TrackingNo| string| 是 | 退货单快递单号 |
| TrackingCompanySysNo| int | 是 | 快递公司系统编码 |
| TrackingRemark| string| 是 | 快递备注 |
| TrackingFileUrlList | array string | 否 | 快递凭证图片 |




> #### 应答_数据_ {#请求数据}

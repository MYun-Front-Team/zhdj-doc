# 核销CPS回填订单

##### _【功能说明】_ {#【功能说明】}

核销CPS回填订单

_**【应用场景】**_
核销CPS回填订单


_**【接口地址】**_
http://ip:port/OrderAction/FLOrder/ConfirmSourceFLOrderCode
> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ConfirmItems|array[ConfirmItem] | 否 | 核销单明细 |
| IsCorrect| int| 是 | 是否正确|


> #### ConfirmItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo|int | 否 | 订单系统编码|
| IsCorrect| int| 是 | 是否正确|




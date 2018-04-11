# 获取订单券码 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

获取订单券码

_**【应用场景】**_

获取订单券码

_**【接口地址】**_

[http://ip:port/OrderQuery/](http://ip:port/HMAction/River/AddRiver)Order[/G](http://ip:port/HMAction/River/AddRiver)etOrderCouponCodeList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 是 | 订单系统编码 |

> #### 应答_数据（数组）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CouponCodeSysNo | int | 是 | 系统编码 |
| CouponCode | string | 是 | 券码 |
| TotalCount | int | 是 | 总数 |
| UsedCount | int | 是 | 已使用数量 |
| EffectiveDate | string | 是 | 有效期 |
| IfOverdueStauts | int | 是 | 是否失效用（0未失效1已失效） |




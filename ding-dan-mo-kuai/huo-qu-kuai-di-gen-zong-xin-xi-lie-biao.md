# 获取快递跟踪信息列表 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

获取快递跟踪信息列表

_**【应用场景】**_

获取快递跟踪信息列表

注：1、调用第三方接口原样返回；

2、需根据快递公司系统编码匹配到快递公司的Code；

_**【接口地址】**_

[http://ip:port/OrderQuery/](http://ip:port/HMAction/River/AddRiver)Order[/G](http://ip:port/HMAction/River/AddRiver)etExpressMessageList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TrackingCompanySysNo | int | 是 | 快递公司系统编码 |
| TrackingNo | string | 是 | 单号 |

> #### 应答_数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| status | string | 是 | 状态，正常为0 |
| msg | string | 是 | 信息，正常为ok |
| result | object | 是 | 结果 |

#### result说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeliveryStatus | int | 是 | 物流状态：1在途 2派件中 3已签收 4派送失败（拒签等） |
| list | array object | 是 | 跟踪信息列表 |

#### list说明（数组） {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| time | string | 是 | 时间 |
| status | string | 是 | 说明 |




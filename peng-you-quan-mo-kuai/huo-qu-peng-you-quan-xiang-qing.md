# 获取朋友圈详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取朋友圈详情

_**【应用场景】**_

获取朋友圈详情。

_**【接口地址】**_

[http://ip:port/MomentsQuery/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Moments](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/G](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etMomentsBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MomentsSysNo | int | 否 | 系统编码 |
| Limit | array | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
|  |  | 是 | 基础字段 |
|  |  | 否 | 统计字段 |




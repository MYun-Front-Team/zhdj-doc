# 获取职位详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取职位详情

_**【应用场景】**_

获取职位详情

_**【接口地址】**_

[http://ip:port/RecruitQuery/Position/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)PositionBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionSysNo | int | 否 | 职位系统编码 |
| Limit | array | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionBase | object | 是 | 基础字段 |
| PositionStatistic | object | 否 | 统计字段 |




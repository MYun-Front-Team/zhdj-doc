# 获取活动详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取活动详情

_**【应用场景】**_

获取活动详情。

注意：如该人未曾阅读，插入一条人员足迹，标记已读。

_**【接口地址】**_

[http://ip:port/ActivityQuery/Activity/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ActivityBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivitySysNo | int | 否 | 系统编码 |
| Limit | array | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
|  |  | 是 | 基础字段 |
|  |  | 否 | 统计字段 |

#### ActivityPersonList说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivityPersonSysNo | int | 是 | 系统编码 |
| PersonPost | string | 否 | 岗位 |
| ActivityPersonPerson | object | 是 | 人员实体 |
| PersonStatus | int | 是 | 状态：1报名, 10签到，11请假 |
| SignTime | string | 是 | 签到时间 |
| SignPlace | string | 否 | 签到地点（定位） |
| Longitude | decimal | 否 | 经度（定位） |
| Latitude | decimal | 否 | 纬度（定位） |
| Reason | string | 否 | 请假原因 |
| Remark | string | 否 | 备注 |




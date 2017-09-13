# 获取活动人员记录 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取活动人员记录

_**【应用场景】**_

获取活动人员记录

_**【接口地址】**_

[http://ip:port/ActivityQuery/Activity/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ActivityPersonList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivitySysNo | int | 是 | 活动系统编码 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

#### ActivityPersonList说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivityPersonSysNo | int | 是 | 人员足迹系统编码 |
| PersonPost | string | 否 | 岗位（冗余） |
| PersonDepartment | string | 否 | 部门（冗余） |
| ActivityPersonPerson | object | 是 | 人员实体 |
| PersonStatus | int | 是 | 状态：1报名, 10签到，11请假 |
| SignTime | string | 是 | 签到时间 |
| SignPlace | string | 否 | 签到地点（定位） |
| Longitude | decimal | 否 | 经度（定位） |
| Latitude | decimal | 否 | 纬度（定位） |
| Reason | string | 否 | 请假原因 |
| ~~SignSummary~~ | ~~string~~ | ~~否~~ | ~~个人记要~~ |
| ~~SignSummaryTime~~ | ~~string~~ | ~~否~~ | ~~个人记要时间~~ |
| Remark | string | 否 | 备注 |




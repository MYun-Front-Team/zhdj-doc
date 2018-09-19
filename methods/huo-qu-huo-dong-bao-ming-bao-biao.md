# 获取活动报名报表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取活动报名报表

_**【应用场景】**_

获取活动报名报表

_**【接口地址】**_

[http://ip:port/ActivityQuery/Activity/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ActivityPersonReportList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivitySysNoList | array\[int\] | 否 | 活动列表 |
| CPSSysNoList | array\[int\] | 否 | 渠道列表 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 描述 |
| :--- | :--- | :--- |
| ActivityPersonSysNo | int | 主键 |
| ActivitySysNo | int | 活动id |
| PersonSysNo | int | 人员id |
| ActivityTitle | string | 活动标题 |
| ActivityStartTime | datetime | 活动起始时间 |
| ActivityEndTime | datetime | 活动结束时间 |
| CPSSysNo | int | 渠道编码 |
| CPSName | string | 渠道名称 |
| CPSCode | string | 渠道编号 |
| CellPhoneNo | string | 手机号 |
| RealName | string | 姓名 |
| BirthDay | datetime | 生日（预产期） |
| PCDCode | string | 省市区编码 |
| PCDDescription | string | 省市区描述 |
| SignUpTime | datetime | 报名时间 |

####  {#应答数据-（巡河记录数组）}




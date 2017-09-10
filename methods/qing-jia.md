# 请假 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

活动模块-请假

_**【应用场景】**_

活动报名后才能请假。（该接口不支持未报名也可请假的功能场景）底层需通过InUserSysNo找到Person实体，冗余信息到人相关字段中。

_**【接口地址】**_

[http://ip:port/ActivityAction/Activity/](http://ip:port/HMAction/River/AddRiver)LeaveActivity

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivitySysNo | int | 是 | 活动系统编码 |
| Reason | string | 是 | 请假原因 |
| SignTime | string | 是 | 请假时间 |
| SignPlace | string | 否 | 请假地点（定位） |
| Longitude | decimal | 否 | 经度（定位） |
| Latitude | decimal | 否 | 纬度（定位） |
| Remark | string | 否 | 备注 |




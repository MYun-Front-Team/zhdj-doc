# 签到 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

活动模块-签到

_**【应用场景】**_

活动报名后才能签到。（该接口不支持未报名也可签到的功能场景）

底层需通过InUserSysNo找到Person实体，冗余信息到人相关字段中。

如果有请假数据，需清空。

积分备注：签到动作（枚举=8）预埋积分赠送逻辑。

_**【接口地址】**_

[http://ip:port/ActivityAction/Activity/](http://ip:port/HMAction/River/AddRiver)SignInActivity

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivitySysNo | int | 是 | 活动系统编码 |
| SignTime | string | 是 | 签到时间 |
| SignPlace | string | 否 | 签到地点（定位） |
| Longitude | decimal | 否 | 经度（定位） |
| Latitude | decimal | 否 | 纬度（定位） |
| Remark | string | 否 | 备注（累加格式：内容+时间+人） |




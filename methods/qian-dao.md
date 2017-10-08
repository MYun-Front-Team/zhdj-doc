# 签到 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

活动模块-签到

_**【应用场景】**_

功能1：IsNeedSignUp=0或空，可直接签到，跳过报名环节；

功能2：SignInPersonSysNo&gt;0，则提供代签功能；

功能3：先报名，后签到。

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
| IsNeedSignUp | int | 否 | 是否需要报名：0否，1是 |
| SignInPersonSysNo | int | 否 | 需代签人员系统编码 |




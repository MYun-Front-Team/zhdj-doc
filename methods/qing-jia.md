# 请假 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

活动模块-请假

_**【应用场景】**_

功能1：IsNeedSignUp=0或空，可直接请假，跳过报名环节；

功能2：SignInPersonSysNo&gt;0，则提供代请假功能；

功能3：先报名，后请假；

功能4：是否撤销请假，返回的状态根据“是否需要报名”字段，需要报名则回到已报名状态，不需要报名则初始化状态；

底层需通过InUserSysNo找到Person实体，冗余信息到人相关字段中。

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
| IsNeedSignUp | int | 否 | 是否需要报名：0否，1是 |
| SignInPersonSysNo | int | 否 | 需代请假人员系统编码 |
| IsRemove | int | 否 | 是否撤销：0否，1是 |
| CPSSysNo | int | 否 | CPS渠道编码 |




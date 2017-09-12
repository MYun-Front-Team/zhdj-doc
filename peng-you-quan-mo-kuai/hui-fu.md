# 回复 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

朋友圈模块-回复

_**【应用场景】**_

朋友圈模块-回复。

注：通过UserSysNo匹配人员信息到FromPerson，并记录表中状态、时间等信息。

_**【接口地址】**_

[http://ip:port/MomentsAction/Moments/Add](http://ip:port/HMAction/River/AddRiver)Moments

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MomentsSysNo | int | 是 | 朋友圈记录系统编码 |
| ToPersonSysNo | int | 是 | 接收人人员编码（非UserSysNo） |
| SignContent | string | 是 | 回复内容 |
| SignPlace | string | 否 | 定位地址 |
| Longitude | decimal | 否 | 经度 |
| Latitude | decimal | 否 | 纬度 |




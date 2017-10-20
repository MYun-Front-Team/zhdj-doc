# 回复 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

朋友圈模块-回复

_**【应用场景】**_

朋友圈模块-回复。

注：通过UserSysNo匹配人员信息到FromPerson，并记录表中状态、时间等信息。

积分备注：回复动作（枚举=14）预埋积分赠送逻辑。

_**【接口地址】**_

[http://ip:port/MomentsAction/Moments/SetMomentsReply](http://ip:port/HMAction/River/AddRiver)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MomentsSysNo | int | 是 | 朋友圈记录系统编码 |
| ToPersonSysNo | int | 是 | 接收人人员编码（非UserSysNo） |
| SignContent | string | 是 | 回复内容 |
| SignPlace | string | 否 | 定位地址 |
| Longitude | decimal | 否 | 经度 |
| Latitude | decimal | 否 | 纬度 |

#### _应答数据_ {#应答数据-}

#### MonentsPersonList实体的单个对象 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MonentsPersonSysNo | int | 是 | 人员足迹系统编码 |
| FromPerson | object | 是 | 发表人员实体 |
| ToPerson | object | 是 | 接收人员实体 |
| IsReaded | int | 是 | 是否已读：0否，1是 |
| PersonStatus | int | 是 | 状态：0发布定位，1浏览，2点赞，3转发，4分享 ，5回复 |
| SignCount | int | 是 | 足迹次数 |
| SignTime | string | 是 | 最近足迹时间 |
| SignPlace | string | 否 | 最近足迹地点（定位） |
| SignContent | string | 否 | 足迹内容（回复） |
| Longitude | decimal | 否 | 经度（定位） |
| Latitude | decimal | 否 | 纬度（定位） |
| Remark | string | 否 | 备注 |
| Moments | object | 否 | 朋友圈记录实体对象（只有在获取未读列表中返回） |




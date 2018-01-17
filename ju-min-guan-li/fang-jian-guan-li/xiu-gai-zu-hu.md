# 修改房间租户 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改房间租户

_**【应用场景】**_

修改房间租户

（图片都在Person实体中，见基础模块-获取人员详情）

_**【接口地址】**_

[http://ip:port/ResidentAction/Room/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditRoomTenant

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RoomSysNo | int | 是 | 房间系统编码 |
| Resident | object | 是 | 居民实体 |
| IsTenant | int | 是 | 是否租户 |
| IsLive | int | 是 | 是否居住在该房间 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




# 新增房间 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增房间

_**【应用场景】**_

新增房间

_**【接口地址】**_

[http://ip:port/ResidentAction/Room/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddRoom

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HouseSysNo | int | 是 | 房屋系统编码 |
| RoomNo | string | 否 | 房间编号 |
| RoomName | string | 是 | 房间名称 |
| RoomArea | decimal\(18,2\) | 否 | 房间面积 |
| RoomOrientation | string | 否 | 房间朝向 |
| RoomPurpose | int | 否 | 房间用途：0自用，1出租 |
| RoomTenantNum | int | 否 | 承租户数量 |
| RoomPermitNum | int | 否 | 办证数量 |
| Propertys | array object | 否 | 房间属性列表 |
| TenantList | array object | 否 | 租户列表 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RoomSysNo | int | 是 | 系统编码 |

#### Tenant说明_ _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Person | object | 是 | 人员 |
| IsTenant | int | 是 | 是否租户 |
| IsLive | int | 是 | 是否居住在该房间 |




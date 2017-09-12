# 获取党员先锋站详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取党员先锋站详情

_**【应用场景】**_

获取党员先锋站详情

_**【接口地址】**_

[http://ip:port/PartyQuery/Station/GetP](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)artyStationBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StationSysNo | int | 是 | 系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StationSysNo | int | 是 | 系统编码 |
| StationName | string | 是 | 名称 |
| StationAddress | string | 是 | 地址 |
| StationContent | string | 否 | 描述 |
| Remark | string | 否 | 备注 |
| Longitude | decimal | 是 | 经度 |
| Latitude | decimal | 是 | 纬度 |




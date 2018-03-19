# 新增党员先锋站 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增党员先锋站

_**【应用场景】**_

新增党员先锋站

_**【接口地址】**_

[http://ip:port/PartyAction/Station/AddP](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)artyStation

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 数据范围树编码 |
| StationName | string | 是 | 名称 |
| StationAddress | string | 是 | 地址 |
| StationContent | string | 否 | 描述 |
| Remark | string | 否 | 备注 |
| Longitude | decimal | 是 | 经度 |
| Latitude | decimal | 是 | 纬度 |
| StationPathList | array string | 否 | 图片Path路径列表 |
| StationMaster| string | 否 | 先锋站负责人 |
| StationMasterPhone| string | 否 | 先锋站负责人电话 |



> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StationSysNo | int | 是 | 系统编码 |




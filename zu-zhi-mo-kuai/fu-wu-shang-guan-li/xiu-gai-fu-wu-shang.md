# 修改服务商 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改服务商

_**【应用场景】**_

修改服务商

_**【接口地址】**_

[http://ip:port/OrganizationAction/Servicer/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditServicer

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ServicerSysNo | int | 是 | 系统编码 |
| ServicerType | int | 否 | 服务商类型（行业枚举） |
| ServicerClassSysNo | int | 否 | 服务商类别系统编码（类目树） |
| ServicerLevelSysNo | int | 否 | 服务商等级系统编码 |
| ServicerName | string | 否 | 服务商名称 |
| ServicerShortName | string | 否 | 简称 |
| ServicerTel | string | 否 | 服务商联系电话 |
| ServicerDesc | string | 否 | 服务商描述 |
| ServicerMaster | string | 否 | 服务商负责人 |
| ServicerPost | string | 否 | 服务商负责人岗位 |
| ServicerPerson | string | 否 | 服务商联系人 |
| ServicerPersonPhone | string | 否 | 服务商联系人电话 |
| ServicerPersonPost | string | 否 | 服务商联系人岗位 |
| ContractAddress | string | 否 | 联系地址 |
| Longitude | decimal\(18,2\) | 否 | 经度 |
| Latitude | decimal\(18,2\) | 否 | 纬度 |
| ServicerLogoPathList | array string | 否 | 服务商Logo的路径列表 |
| Remar1| string | 否（可选配置） | 备注1|
| Remar2| string | 否（可选配置） | 备注2|
| Remar3| string | 否（可选配置） | 备注3|





> #### _应答数据 _ {#应答数据-（巡河记录数组）}




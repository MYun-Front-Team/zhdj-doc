# 新增服务商 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增服务商

_**【应用场景】**_

新增服务商

注：ServicerTel必填，一旦服务商启用后创建账户和账号，并分配权限角色；

_**【接口地址】**_

[http://ip:port/OrganizationAction/Servicer/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddServicer

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| ServicerType | int | 是 | 服务商类型（行业枚举） |
| ServicerClassSysNo | int | 否（可选配置） | 服务商类别系统编码（类目树） |
| ServicerLevelSysNo | int | 否（可选配置） | 服务商等级系统编码 |
| ServicerStatus | int | 否（可选配置） | 状态：0待发展，10正常，11终止 |
| ServicerName | string | 是 | 服务商名称 |
| ServicerShortName | string | 否（可选配置） | 简称 |
| ServicerTel | string | 是 | 服务商联系电话 |
| ServicerDesc | string | 否（可选配置） | 服务商描述 |
| ServicerMaster | string | 否（可选配置） | 服务商负责人 |
| ServicerPost | string | 否（可选配置） | 服务商负责人岗位 |
| ServicerPerson | string | 否（可选配置） | 服务商联系人 |
| ServicerPersonPhone | string | 否（可选配置） | 服务商联系人电话 |
| ServicerPersonPost | string | 否（可选配置） | 服务商联系人岗位 |
| ContractAddress | string | 否（可选配置） | 联系地址 |
| Longitude | decimal\(18,2\) | 否（可选配置） | 经度 |
| Latitude | decimal\(18,2\) | 否（可选配置） | 纬度 |
| ServicerLogoPathList | array string | 否（可选配置） | 服务商Logo的路径列表 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ServicerSysNo | int | 是 | 服务商系统编码 |




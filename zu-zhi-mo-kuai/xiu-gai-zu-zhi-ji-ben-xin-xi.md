# 修改组织基本信息 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改组织基本信息

_**【应用场景】**_

修改组织基本信息

注：从UserSysNo找到的Person，必须存在于该组织才能修改组织信息；

_**【接口地址】**_

[http://ip:port/OrganizationAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Organization](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditOrganization

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| OrganizationName | string | 否 | 组织名称 |
| OrganizationShortName | string | 否 | 组织简称 |
| OrganizationTel | string | 否 | 组织联系电话 |
| OrganizationDesc | string | 否 | 组织描述 |
| OrganizationMaster | string | 否 | 组织负责人 |
| OrganizationPost | string | 否 | 组织负责人岗位 |
| OrganizationPerson | string | 否 | 组织联系人 |
| OrganizationPersonPhone | string | 否 | 组织联系人电话 |
| OrganizationPersonPost | string | 否 | 组织联系人岗位 |
| ContractAddress | string | 否 | 联系地址 |
| Longitude | decimal（18，10） | 否 | 经度 |
| Latitude | decimal（18，10） | 否 | 纬度 |
| OrganizationLogoPathList | array string | 否 | 组织Logo的路径列表 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




# 新增组织 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/OrganizationAction/Organization/AddOrganization](http://ip:port/OrganizationAction/Organization/AddOrganization)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationType | int | 是 | 组织类型 |
| OrganizationClassSysNo | int | 否 | 组织类别 |
| OrganizationName | string | 是 | 组织名称 |
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
| DataRangeSysNo | int | 否 | 所属区域 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织编码 |




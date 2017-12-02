# 获取快递公司列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取快递公司列表

_**【应用场景】**_

获取快递公司列表

注：如果该组织没有配置快递公司，则获取平台方组织下的快递列表，并标记所有者；

_**【接口地址】**_

[http://ip:port/UMQuery/TrackingCompany/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)TrackingCompanyList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围树编码（店铺树） |
| TrackingCompanyTypeList | int | 否 | 类型：0快递，1物流 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TrackingCompanySysNo | int | 是 | 系统编码 |
| TrackingCompanyType | string | 是 | 类型：0快递，1物流 |
| TrackingCompanyCode | int | 否 | 快递公司代码 |
| TrackingCompanyName | string | 是 | 快递公司名称 |
| TrackingCompanyLogoUrl | string | 否 | Logo |
| IsCreator | int | 是 | 是否所有者：0否，1是 |




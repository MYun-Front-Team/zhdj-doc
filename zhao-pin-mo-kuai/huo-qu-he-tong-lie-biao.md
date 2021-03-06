# 获取合同列表

##### _【功能说明】_ {#【功能说明】}

获取合同列表

_**【应用场景】**_

获取合同列表

_**【接口地址】**_

[http://ip:port/RecruitQuery/Contract/GetContractList](http://ip:port/RecruitQuery/Contract/GetContractList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员编码 |
| PositionType | int | 是 | 岗位类型 |
| OrganizationSysNo | int | 是 | 商家组织号 |
| ShopSysNo | int | 是 | 店铺编码 |
| ContractStatusList | array int | 是 | 合同状态（0待签 10已签 11拒签） |
| StartContractStart | datetime | 是 | 起始合同开始 |
| EndContractStart | datetime | 是 | 终止合同开始 |
| StartContractEnd | datetime | 是 | 起始合同结束 |
| EndContractEnd | datetime | 是 | 终止合同结束 |
| KeyWord | string | 是 | 关键字 |
| InvitePersonSysNo | int | 是 | 交付人编码 |
| RecruitCertificateSysNo | int | 否 | 招聘签约主体 |

#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ContractSysNo | int | 是 | 合同系统编码 |
| PersonSysNo | int | 是 | 人员编码 |
| RealName | string | 是 | 人员名称 |
| CellPhoneNo | string | 是 | 手机号 |
| OrganizationSysNo | int | 是 | 商家组织号 |
| SellerName | string | 是 | 商家名称 |
| DataRangeSysNo | int | 是 | 店铺范围编码 |
| ShopSysNo | int | 是 | 店铺编码 |
| ShopName | string | 是 | 店铺名称 |
| PositionSysNo | int | 是 | 岗位编码 |
| PositionName | string | 是 | 岗位名称 |
| SourceFromSysNo | int | 是 | 来源系统编码 |
| SourceFromType | int | 是 | 来源类型 |
| ModuleFromSysNo | int | 是 | 来源模块编码 |
| InvitePersonSysNo | int | 是 | 交付人编码 |
| InvitePersonRealName | string | 是 | 交付人名称 |
| ContractStatus | int | 是 | 合同状态（0待签 10已签 11拒签） |
| ContractStart | datetime | 是 | 合同开始 |
| ContractEnd | datetime | 是 | 合同结束 |
| CreateTime | datetime | 是 | 创建时间 |
| RecruitServerSysNo | int | 否 | 招聘服务商 |
| RecruitServerName | string | 否 | 招聘服务商名称 |
| RecruitCertificateSysNo | int | 否 | 招聘签约主体 |
| RecruitCertificateName | string | 否 | 招聘签约主体名称 |




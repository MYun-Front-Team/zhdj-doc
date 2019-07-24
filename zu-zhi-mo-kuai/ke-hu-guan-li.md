# 客户模块-字段说明 {#新增河流}

> #### CustomerBase基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CustomerSysNo | int | 是 | 客户系统编码 |
| CustomerLevelSysNo | int | 否 | 客户等级系统编码 |
| CustomerStatus | int | 是 | 状态：0待发展，10正常，11终止 |
| CustomerName | string | 是 | 客户名称 |
| CustomerShortName | string | 是 | 简称 |
| CustomerTel | string | 否 | 客户联系电话 |
| CustomerDesc | string | 否 | 客户描述 |
| CustomerMaster | string | 否 | 客户负责人 |
| CustomerPost | string | 否 | 客户负责人岗位 |
| CustomerPerson | string | 否 | 客户联系人 |
| CustomerPersonPhone | string | 否 | 客户联系人电话 |
| CustomerPersonPost | string | 否 | 客户联系人岗位 |
| ContractAddress | string | 否 | 联系地址 |
| Longitude | decimal\(18,2\) | 否 | 经度 |
| Latitude | decimal\(18,2\) | 否 | 纬度 |
| CustomerLogoPathList | array string | 否 | 客户Logo的路径列表 |
| CustomerLogoUrlList | array string | 否 | 客户Logo的Url列表 |
| CustomerPersonSysNo | string | 否 | 客户老板系统编码 |
| CustomerPersonFileUrlList | array string | 否 | 客户老板头像 |
| CustomerPersonFileUrlList | array string | 否 | 客户老板头像 |
| CustomerPCDCode | string | 否 | 客户省市区 |
| CustomerPCDDescription | string | 否 | 客户省市区 |
| CustomerBirthDay | string | 否 | 客户生日 |
| TagList | array object | 否 | 标签列表（说明见通用） |
| IsPartner | int | 是 | 是否合伙人 |
| CustomerDoctorPersonSysNo | int | 否 | 促销员\医生编码 |
| CustomerDoctorPersonName | string | 否 | 促销员\医生名称 |
| HospitalOrgSysNo | int | 否 | 所属医院\机构编码 |
| HospitalOrgName | string | 否 | 所属医院\机构 |
| AgentPersonSysNo | int | 否 | 渠道经理编码 |
| AgentPersonName | string | 否 | 渠道经理名称 |
| PCDDataRangeSysNo | int | 否 | 所属机构的区域编码 |
| PCDDataRangeName | string | 否 | 所属机构的区域 |
| CustomerSalesman | string | 否 | 业务员 |
| PersonSysNo | int | 否 | 人员编码 |
| UseInvitation| int | 否 | 已使用邀请码 |
| NoUseInvitation| int | 否 | 未使用邀请码 |
| PersonName| int | 否 |人员昵称|
| RealName| int | 否 |人员姓名|
| InvitationCode| string| 否 | 邀请码 |
| FatherPersonName| string| 否 | 邀请人 |
| HelpMemberId| string| 否 |辅助id |
| CPSCode| string| 否 |客户来源三方cps编号 |
| CPSSysNo | int | 否 | 客户来源三方cps编码|
| CustomerManagers | array[CustomerManager] | 否 | 客户经理/顾问|




> #### CustomerStatistic统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TeamCount| int | 否 |团队数|
| LJPoint| decimal | 否 |蓝晶数|
| LANPointsIsEnable| int | 否 | 客户蓝晶账号是否启用|





> #### CustomerManager 客户经理/顾问

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ManagerName| string | 否 |顾问名称|
| ManagerType| int | 否 |类型（1顾问 2经理）|
| ManagerSysNo| int | 否 |顾问系统编码|

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### Query查询字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| CustomerSysNo | int | 否 | 客户系统编码 |
| CustomerStatusList | Array\[int\] | 否 | 状态：0待发展，10正常，11终止 |
| KeyWord | string | 否 | 关键字（名称/负责人/联系人/电话） |
| CustomerLevelSysNoList | Array\[int\] | 否 | 客户等级 |
| TagSysNoList | Array\[int\] | 否 | 客户标签 |
| CustomerDoctorPersonName | string | 否 | 促销员\医生 |
| HospitalOrgName | string | 否 | 所属医院\机构 |
| AgentPersonSysNoList | array\[int\] | 否 | 所属渠道经理编码 |
| PCDDataRangeSysNoList | array\[int\] | 否 | 所属机构区域 |
| CustomerSalesman | string | 否 | 业务员 |
| StartCustomerBirthDay | string | 否 | 开始客户生日 |
| EndCustomerBirthDay | string | 否 | 结束客户生日 |
| CustomerPCDDescription | string | 否 | 客户省市区 |
| IfHasCustomerPersonPhone | array[int]| 否 | 是否有电话（1有 0无）| 
| StartCreateTime| string | 否 | 开始注册时间 |
| EndCreateTime| string | 否 | 结束注册时间|
| CustomerManagerPersonSysNo | int | 否 | 客户经理人员


系统编码 |




> #### Limit限制字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowDefaultAddress | int | 否 | 是否显示客户所属组织的默认地址（当原客户地址没有维护时有效） |
| IsShowTagList | int | 否 | 是否显示标签列表 |
| IsShowHelpMemberId | int | 否 | 是否显示辅助ID |
| IsShowCustomerStatistic | int | 否 | 是否显示统计字段 |
| IsShowCustomerManager| int | 否 | 是否显示客户经理 |


#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |





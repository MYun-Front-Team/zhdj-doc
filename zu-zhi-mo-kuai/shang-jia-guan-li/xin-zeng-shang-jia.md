# 新增商家 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增商家

_**【应用场景】**_

新增商家

注：组织系统编码=0则先使用Register判断是否需要注册或原来就已经存在组织；

注：邀请码逻辑暂缺；

_**【接口地址】**_

[http://ip:port/OrganizationAction/Seller/AddS](http://ip:port/OrganizationAction/Customer/AddCustomer)eller

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| ~~Register~~ | ~~object~~ | ~~否~~ | ~~注册实体（见注册接口）~~ |
|  |  |  |  |
| SellerType | int | 否（可选配置） | 商家类型 |
| SellerClassSysNo | int | 否（可选配置） | 商家类别系统编码（类目树） |
| SellerName | string | 是 | 商家名称 |
| SellerShortName | string | 否（可选配置） | 简称 |
| SellerTel | string | 否（可选配置） | 商家联系电话 |
| SellerDesc | string | 是 | 商家描述 |
| SellerMaster | string | 否（可选配置） | 商家负责人 |
| SellerPost | string | 否（可选配置） | 商家负责人岗位 |
| SellerIDCard | string | 否（可选配置） | 商家负责人身份证 |
| SellerGender | int | 否（可选配置） | 商家负责人性别：1男，2女 |
| SellerPerson | string | 否（可选配置） | 商家联系人 |
| SellerPersonPhone | string | 否（可选配置） | 商家联系人电话 |
| SellerPersonPost | string | 否（可选配置） | 商家联系人岗位 |
| PCDCode | string | 否（可选配置） | 省市区代码 |
| PCDDescription | string | 否（可选配置） | 省市区描述 |
| ContractAddress | string | 否（可选配置） | 联系地址 |
| Longitude | decimal\(18,2\) | 否（可选配置） | 经度 |
| Latitude | decimal\(18,2\) | 否（可选配置） | 纬度 |
| Remark | string | 否（可选配置） | 备注 |
| IDCardPathList | array string | 否（可选配置） | 身份证Path路径列表 |
| LicensePathList | array string | 否（可选配置） | 营业执照Path路径列表 |
| InvitationCode | string | 否（可选配置） | 邀请码 |
| SellerLogoPathList | array string | 否（可选配置） | 商家Logo的Path路径列表 |
| CategorySysNoList | array int | 否（可选配置） | 商家行业类型编码列表 |
| SellerFinancePerson| string | 否 |财务联系人 |
| SellerFinancePhone| string | 否 |财务联系人电话 |
| ParkSysNo| int | 否 |注册地址（园区） |
| IfHasPhysicalStore| int | 否 |是否有实体 |
| IfHasInternetStore| int | 否 |是否有网店 |
| ScaleType| int | 否 |规模（端定义） |
| RegistrationTime| datetime| 否 |注册时间 |
| PromisesTax| decimal| 否 |承诺税收 |
| RegisteredCapital| decimal| 否 |注册资金 |
| CreditCode| decimal| 否 |信用编码 |
| InternetStoreUrl| string | 否 |网店地址 |
 |InParkDate| datetime | 否 |入驻时间 |
|InParkStatus| int | 否 |状态（潜在客户，已入驻，已签出） |
|LicenseType| string | 否 |营业执照类型 |
|LicenseAddress| string | 否 |营业执照地址 |
|LicenseStartDate| datetime | 否 |营业期限开始|
|LicenseEndDate| datetime | 否 |营业期限结束|
|OutParkDate| datetime | 否 |迁出时间 |
|OutParkRemark| string | 否 |迁出备注|
| ServicePersonSysNo| int | 否 |默认客服编码 |
|ContractCode| string | 否 |合同编号|
| ObjectFileList| array File| 否（可选配置） | 附件 |
| AutoAudit| int | 否 |是否自动审核（1是 0否）|
| IsShowInCommission| int| 否 | 是否在抢工佣金推送列表显示 |
| RecruitNeedPlatAudit| int | 否 |发布岗位是否需要平台审核|
|BackMoneyDay1| int | 否 |回款日期1(号)|
|BackMoneyDay2| int | 否 |回款日期2(号)|
|OutMoneyDay1| int | 否 |发薪日期1(号)|
|OutMoneyDay2| int | 否 |发薪日期2(号)|


#### File说明 {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FileTitle| string| 是 | 文件名称 |
| FilePath| string| 是 | 文件地址 |










#### _应答数据 _ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SellerSysNo | int | 是 | 系统编码 |




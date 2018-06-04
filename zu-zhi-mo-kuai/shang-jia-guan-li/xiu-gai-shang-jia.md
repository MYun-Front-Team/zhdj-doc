# 修改商家 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改商家

_**【应用场景】**_

修改商家

_**【接口地址】**_

[http://ip:port/OrganizationAction/Seller/EditS](http://ip:port/OrganizationAction/Customer/AddCustomer)eller

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SellerSysNo | int | 是 | 商家系统编码 |
| SellerName | string | 否 | 商家名称 |
| SellerShortName | string | 否 | 简称 |
| SellerTel | string | 否 | 商家联系电话 |
| SellerDesc | string | 否 | 商家描述 |
| SellerMaster | string | 否 | 商家负责人 |
| SellerPost | string | 否 | 商家负责人岗位 |
| SellerIDCard | string | 否 | 商家负责人身份证 |
| SellerGender | int | 否 | 商家负责人性别：1男，2女 |
| SellerPerson | string | 否 | 商家联系人 |
| SellerPersonPhone | string | 否 | 商家联系人电话 |
| SellerPersonPost | string | 否 | 商家联系人岗位 |
| PCDCode | string | 否 | 省市区代码 |
| PCDDescription | string | 否 | 省市区描述 |
| ContractAddress | string | 否 | 联系地址 |
| Longitude | decimal\(18,2\) | 否 | 经度 |
| Latitude | decimal\(18,2\) | 否 | 纬度 |
| Remark | string | 否 | 备注 |
| IDCardPathList | array string | 否 | 身份证Path路径列表 |
| LicensePathList | array string | 否 | 营业执照Path路径列表 |
| SellerLogoPathList | array string | 否 | 商家Logo的Path列表 |
| CategorySysNoList | array int | 否 | 商家行业类型编码列表 |
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




#### _应答数据 _ {#应答数据-}




# 新增商家（无组织版） {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增商家

_**【应用场景】**_

新增商家

注：先使用Register判断是否需要注册或原来就已经存在组织；

注：邀请码逻辑暂缺；

_**【接口地址】**_

[http://ip:port/OrganizationAction/Seller/AddS](http://ip:port/OrganizationAction/Customer/AddCustomer)eller2

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ~~OrganizationSysNo~~ | ~~int~~ | ~~是~~ | ~~组织系统编码~~ |
| Register | object | 否 | 注册实体（见注册接口） |
|  |  |  |  |
| SellerType | int | 否（可选配置） | 商家类型（行业枚举） |
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
|ContractCode| string | 否 |合同编号|
| AutoAudit| int | 否 |是否自动审核（1是 0否）|
| RecruitNeedPlatAudit| int | 否 |发布岗位是否需要平台审核|
| PostSysNo| int | 否 |职位编码 |








#### _应答数据 _ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SellerSysNo | int | 是 | 商家系统编码 |
| OrganizationSysNo | int | 是 | 组织系统编码 |




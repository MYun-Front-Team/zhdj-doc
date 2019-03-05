# 商家模块-字段说明 {#新增河流}

> #### SellerBase基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| SellerSysNo | int | 是 | 商家系统编码 |
| SellerType | int | 否 | 商家类型（行业枚举） |
| SellerClassSysNo | int | 否 | 商家类别系统编码（类目树） |
| SellerClassName | string | 否 | 商家类别名称 |
| SellerLevelSysNo | int | 否 | 商家等级系统编码 |
| SellerLevelName | string | 否 | 商家等级名称 |
| AuditStatus | int | 是 | 审核状态：0待审核，10审核通过，11审核失败 |
| AuditRecord | object | 否 | 审核记录实体 |
| SellerStatus | int | 是 | 商家状态：0未缴费，1已缴费 |
| SellerName | string | 是 | 商家名称 |
| SellerShortName | string | 是 | 简称 |
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
| IDCardUrlList | array string | 否 | 身份证Url路径列表 |
| LicenseUrlList | array string | 否 | 营业执照Url路径列表 |
| SellerLogoPathList | array string | 否 | 商家Logo路径列表 |
| SellerLogoUrlList | array string | 否 | 商家Logo的URL列表 |
| SellerBossPerson | object | 否 | 商家创始人实体（默认联系人） |
| SellerCategoryList | array object | 否 | 商家行业类型列表 |
| SellerMasterPhone| string | 否 | 商家负责人电话 |
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
| ParkName| string | 否 |园区名称 |
|OutParkDate| datetime | 否 |迁出时间 |
|OutParkRemark| string | 否 |迁出备注|
| ServicePersonSysNo| int | 否 |默认客服编码 |
| ServicePersonName| string| 否 |默认客服名称 |
| ServiceCellPhoneNo| string| 否 |默认客服电话 |
| ServiceFileUrlList | array string | 否 | 头像图片列表 |
|ContractCode| string | 否 |合同编号|
| ContractPathList | array string | 否 | 合同路径列表 |
| ContractUrlList | array string | 否 | 合同的URL列表 |
|ActiveStatus| int | 否 |激活状态（0待激活，10启用）|
|InUser| string | 否 |创建人|
|EditUser| string | 否 |编辑人|
| ObjectFileList| array File| 否（可选配置） | 附件 |
| IsShowInCommission| int| 否 | 是否在抢工佣金推送列表显示 |
| RecruitNeedPlatAudit| int | 否 |发布岗位是否需要平台审核|
| RMAReceiverAddress| string| 是 | 退货地址 |
| RMAReceiverName| string| 是 | 退货收货人 |
| RMAReceiverPhone| string| 是 | 退货收货人电话|
|BackMoneyDay1| int | 否 |回款日期1(号)|
|BackMoneyDay2| int | 否 |回款日期2(号)|
|OutMoneyDay1| int | 否 |发薪日期1(号)|
|OutMoneyDay2| int | 否 |发薪日期2(号)|
|IsDisable| int | 否 |是否禁用（1禁用，0启用）|
|SignDate| datetime| 否 |签约日期|
|InvoiceType| int | 否 |开票方式（1专用发票 2普通发票）|
|IfHasTax| int | 否 |是否含税|
|TaxRate| decimal| 否 |税率|
|SalaryTimes| int | 否 |加班时薪倍数|
|SalesManagerPersonSysNo| int | 否 |销售经理|
|SalesManagerDepartmentSysNo| int | 否 |销售部门编码|
|SalesManagerDepartmentName| string| 否 |销售部门|
|RecruitStatus| int | 否 |招聘状态（10进行中，0未开始）|





#### File说明 {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FileTitle| string| 是 | 文件名称 |
| FilePath| string| 是 | 文件地址 |
| FileUrl| string| 是 | 文件地址 |




> #### SellerStatistic统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Wallet | object | 否 | 钱包实体（资金说明） |
| ShopCount| int | 否 |店铺数量 |
| PartTimeJobCount| int | 否 |兼职数量 |
| FullTimeJobCount| int | 否 |全职数量 |


> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### Query查询字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| SellerSysNo | int | 否 | 商家系统编码 |
| AuditStatusList | Array\[int\] | 否 | 审核状态 |
| SellerStatusList | Array\[int\] | 否 | 商家状态 |
| KeyWord | string | 否 | 关键字（名称/负责人/联系人/电话） |
|ScaleTypeList|Array\[int\] | 否 | 企业规模 |
|InParkStatusList|Array\[int\] | 否 | 状态（潜在客户，已入驻，已签出） |
|SellerClassSysNoList|Array\[int\] | 否 | 商家类别系统编码（类目树） |
| ParkSysNo| int | 否 |注册地址（园区） |
| SellerTypeList | array int | 否 | 商家类型（行业枚举） |
| OrganizationSysNoList | array  int | 是 | 组织系统编码 |
| IsShowInCommissionList | array  int | 是 |是否在抢工佣金推送列表显示 |
| SalesManagerPersonSysNo| int | 是 |销售人员 |
| IfHasSalesManagerDepartment| int | 是 |是否有销售部门 |
| RecruitStatusList | array  int | 是 |招聘状态（10进行中，0未开始）|




> #### Limit限制字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IDCardUrlList | int | 否 | 是否显示身份证列表 |
| LicenseUrlList | int | 否 | 是否显示营业执照列表 |
| IsShowWallet | int | 否 | 是否显示钱包 |
| IsShowSellerBossPerson | int | 否 | 是否显示商家创始人 |
| IsShowSellerCategoryList | int | 否 | 是否显示商家行业列表 |
| IsShowObjectFileList | int | 否 | 是否显示附件 |



#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |


#### AuditRecord说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AuditRecordSysNo | int | 是 | 系统编码 |
| AuditDate | string | 是 | 审核时间 |
| AuditRemark | string | 否 | 审核备注 |
| AuditResult | int | 是 | 审核结果：10审核通过，11审核失败 |
| AuditPerson | object | 是 | 审核人实体（简） |




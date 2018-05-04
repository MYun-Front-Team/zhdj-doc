# 新增项目

##### _【功能说明】_ {#【功能说明】}

新增项目

_**【应用场景】**_

新增项目

_**【接口地址】**_

http://ip:port/ParkAction/IndustryProject/AddParkProject

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 企业组织系统编码 |
| ProjectName | string | 否 |项目名称 |
| ProjectType | int | 否 |项目类别 |
| ProjectClassSysNo | int | 否 | 项目分类（枚举） |
| ProjectStatus | int | 否 |项目状态（0潜在，1洽谈，2入住，3长期） |
|SaleType | int | 否 |企业类别（端定义） |
|SaleScale | int | 否 |企业规模（端定义） |
|BusinessScope| string | 否 |主营业务 |
|Investor| string | 否 |投资方 |
|AdmissionType| int | 否 |入驻类型（端定义）|
| ProjectPerson| string | 否 |联系人|
| ProjectPersonPhone| string | 否 |联系电话|
| ConfusingFunds| decimal | 否 |认缴资金|
| RealFunds| decimal | 否 |实缴资金|
| LastTicketFunds| decimal | 否 |上年度开票销售额|
| TicketFunds| decimal | 否 |预计入驻后年开票销售额|
| LastTaxRevenue| decimal | 否 |上年度纳税额|
| TaxRevenue| decimal | 否 |预计入驻后年纳税额|
| OfficeArea| decimal | 否 |办公面积|
| OfficeAddress| string | 否 |办公地址|
| WarehouseAddress| string | 否 |仓库地址|
| OtherInfo| string | 否 |其他所需配套|
| ProjectDesc| string | 否 |项目简介|
| ProjectRecommend| string | 否 |项目推荐人|
| ProjectNegotiation| string | 否 |招商洽谈人|
| WarehouseArea| decimal | 否 |仓库面积|




> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProjectSysNo | int | 是 | 项目系统编码 |



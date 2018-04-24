# 房间管理

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeSysNo | int | 是 | 费用系统编码 |
| FeeType | int | 是 | 费用类型 |
| FeeStatus | int | 否 |缴纳状态（0未缴纳，1部分缴纳，10完成缴纳） |
| NoticeCount | int | 否 |催缴次数 |
| FeeClassSysNo | int | 否 | 费用分类（枚举） |
| StartDate | datetime | 否 | 费用开始时间 |
| EndDate | datetime | 否 | 费用结束时间 |
| ParkSysNo| int | 否 | 园区编码|
| ParkName | string | 否 | 园区名称|
| SellerName | string | 否 |企业名称 |
| OrganizationSysNo | int | 是 | 企业组织系统编码 |
| FeeItems | array FeeItem | 否 |费用详情 |
| FeePayDetails | array FeePayDetail | 否 |缴费记录 |
| RefundDetails | array RefundDetail | 否 |退款记录 |
| TotalFee | decimal | 否 |总费用（FeeItem的TotalFee总计） |
| PaidFee | decimal | 否 |实际支付 |




> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeInfos | array[FeeInfo] | 否 |各个费用类型 |




 #### FeeItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeItemSysNo | int | 否 |费用明细编码 |
| BuildingName | string | 是  | 楼宇名称 |
| ParkRoomName| string | 是  | 房间名称|
|ParkRoomType | int | 是 |房间类型|
| FeeItemType| int | 否 |费用类型（端定义）|
| UnitFee| decimal | 否 |单价|
| Count| decimal | 否 |数量（支持小数点）|
| TotalFee| decimal | 否 |总价（非计算，按照客户填的为准）|
| ItemStartDate| datetime | 否 |开始日期|
| ItemEndDate| datetime | 否 |截止日期|


###FeePayDetail

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeePayDetailSysNo | int | 否 |支付凭着系统编码 |
| PaidFee | decimal | 否 |实际支付 |
| PayTime| datetime | 是 | 缴费时间|
| PayType| int | 是 | 缴费类型（端定义）|
| PaidRemark| string | 是 | 缴费备注|
| PaidFilePathList | array string | 否 |凭证照片 |
| PaidFileUrlList | array string | 否 |凭证照片 |
| PaidPerson| string | 是 | 缴费人|
| AuditStatus| int | 是 | 确认状态（0待确认，10已确认）|


###RefundDetail

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Amount | decimal | 否 |退款金额 |
| Remark | string | 否 |退款理由 |

###FeeInfo
| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeItemType| int | 否 |费用类型（端定义）|
| Amount | decimal | 否 |金额 |



> #### 功能按钮字段 {#请求数据}

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeTypeList |array int | 是 | 费用类型 |
| StartDate | datetime | 否 | 费用开始时间 |
| EndDate | datetime | 否 | 费用结束时间 |
| ParkSysNo| int | 否 | 园区编码|
| KeyWord| string | 否 | 关键字|
| OrganizationSysNo | int | 是 | 企业组织系统编码 |
| FeeStatusList |array int | 否 |缴纳状态（0未缴纳，1部分缴纳，10完成缴纳） |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |






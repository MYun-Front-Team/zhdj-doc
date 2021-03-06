`# 缴费模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentFeeSysNo | int | 是 | 缴费系统编码 |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树编码 |
| PaidName | Nvarchar\(50\) | 是 | 缴费名称 |
| SubPaidClassCode | Nvarchar\(50\) | 是 | 子费种编码\(通用类\) |
| SubPaidClassName | Nvarchar\(50\) | 是 | 子费种名称 |
| AuditStatus | int | 是 | 审核状态：0未提交，1审核中，10审核通过，11审核失败 |
| PaidStatus | int | 是 | 缴费状态：0未开始缴费，1未下载，2已下载 9缴费中，10缴费完成 |
| PaidAmount | decimal\(18,2\) | 是 | 单笔缴费费用 |
| PaidStartDate | string | 否 | 有效期开始时间 |
| PaidEndDate | string | 否 | 有效期结束时间 |
| Remark | string | 否 | 备注 |
| LastAuditRecord | object | 否 | 最新的审核记录 |
| SubmitPerson | object | 否 | 提交人（简版） |
| ToParentRemark | string | 否 | 家长告知 |
| ConfirmStatus | int | 是 | 确认状态：0未提交，1待确认，2部分确认，10全部确认|
| DataRanges| array[DataRange]| 是 | 班级-年级-学校数组 |
| InUser| string | 否 | 创建人 |


> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PayAbleTotalAmount | decimal\(18,2\) | 否 | 应缴总金额 |
| TotalAmount | decimal\(18,2\) | 否 | 总金额 |
| PaidTotalAmount | decimal\(18,2\) | 否 | 已缴总金额 |
| PersonTotalCount | int | 否 | 费用相关总人数 |
| WaitPaidCount | int | 否 | 待缴总人数 |
| PersonPaidCount | int | 否 | 已缴总人数 |

> #### 功能按钮字段 {#请求数据}

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | array  int |否 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称） |
| IsMyFootPrint | int | 否 | 是否显示自己的：0否，1是（不传查全部，传值需通过UserSysNo匹配Person） |
| AuditStatusList | array int | 否 | 审核状态：0未提交，1审核中，10审核通过，11审核失败 |
| PaidStatusList | array int | 否 | 缴费状态：0未开始缴费，1未下载，2已下载 9缴费中，10缴费完成 |
| SubPaidClassCode | string | 是 | 子费种编码\(通用类\) |
| SubmitPersonName | string | 是 | 提交人 |
| StudentFeeSysNo | int | 是 | 缴费系统编码 |
| ConfirmStatusList | int | 是 | 确认状态：0未提交，1待确认，2部分确认，10全部确认|
| ItemConfirmStatus | int | 否| 费用明细确认状态：0待确认，10全部确认，（传ItemDataRangeSysNoList才有效） |
| ItemDataRangeSysNoList | array  int |否 | 费用明细数据范围树枝叶编码列表 |






> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowLastAuditRecord | int | 否 | 是否显示最新审核记录 |
| IsShowPayAbleTotalAmount | int | 否 | 是否显示应缴总金额 |
| IsShowPaidTotalAmount | int | 否 | 是否显示已缴总金额 |
| IsShowPersonTotalCount | int | 否 | 是否显示已缴总人数 |
| IsShowPersonPaidCount | int | 否 | 是否显示未缴总人数 |
| IsShowSubmitPerson | int | 否 | 是否显示提交人 |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}




# 获取退货单详情

##### _【功能说明】_ {#【功能说明】}

获取退货单详情

_**【应用场景】**_

获取退货单详情

_**【接口地址】**_

http://ip:port/OrderQuery/RMA/GetOrderRMABySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RMASysNo | int | 是 | 退货单系统编码 |



> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RMASysNo | int | 是 | 退货单系统编码 |
| RMAType | int | 是 | 退货单类型（1仅退款，2退货/退款） |
| RMAStatus | int | 是 | 退货单状态（1等待卖家同意退货，2等待卖家同意退款，3等待买家退货，4等待卖家确认收货，10退款成功，11退款关闭） |
| OrderSysNo | int | 是 | 订单系统编码 |
| OrganizationFromSysNo | int | 是 | 卖家组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树编码（店铺树） |
| OrganizationToSysNo | int | 是 | 买家组织系统编码 |
| OrderItemSysNo | int | 是 | 订单明细系统编码 |
| Person| Person | 是 | 买家人员|
| RMAReason| string| 是 | 退货理由 |
| Remark | string | 否 | 退货备注 |
| FileUrlList | array string | 否 | 图片列表 |
| SkuSysNo | int | 是 | Sku编码 |
| ProductGroupSysNo| int | 是 | 款编码 |
| ProductGroupName | string | 是 | 款名称 |
| RMAAmount| decimal| 是 | 退款金额 |
| CancelStatus | int | 是 | 取消状态：0正常，10客户已取消|
| AuditStatus | int | 是 | 审核状态：0待审核，10审核通过，11审核失败 |
| AuditRecord | object | 否 | 审核记录实体 |
| CreateTime| datetime| 否 | 申请时间|
| FileThumbnailUrlList | array string | 否 | 缩略图Url列表 |
| RMACount| int | 是 | 数量 |
| UnitPrice| decimal| 是 |单价 |
| OrderAmount| decimal| 是 | 订单金额 |
| GoodBackAuditStatus | int | 是 | 退货审核状态：0待审核，10审核通过，11审核失败 |
| GoodBackAuditRecord| object | 是 | 退货审核记录实体 |
| TrackingNo| string| 是 | 退货单快递单号 |
| TrackingCompanySysNo| int | 是 | 快递公司系统编码 |
| TrackingCompanyName| string| 是 | 快递公司名称 |
| TrackingCompanyCode| string| 是 | 三方快递公司查询码 |
| TrackingRemark| string| 是 | 快递备注 |
| TrackingFileUrlList | array string | 否 | 快递凭证图片 |
| TrackingCompanyName| string| 是 | 快递公司名称 |
| SourceCPSName| string| 是 | 来源 |
| SourceCPSCode| string| 是 | 来源编号 |
| RMAReceiverAddress| string| 是 | 退货地址 |
| RMAReceiverName| string| 是 | 退货收货人 |
| RMAReceiverPhone| string| 是 | 退货收货人电话|



#### AuditRecord说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AuditRecordSysNo | int | 是 | 系统编码 |
| AuditDate | string | 是 | 审核时间 |
| AuditRemark | string | 否 | 审核备注 |
| AuditPerson | object | 是 | 审核人实体（简） |























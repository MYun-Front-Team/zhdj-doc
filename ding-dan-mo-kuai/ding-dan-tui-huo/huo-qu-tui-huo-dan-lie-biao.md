# 获取退货单列表

##### _【功能说明】_ {#【功能说明】}

获取退货单列表

_**【应用场景】**_

获取退货单列表

_**【接口地址】**_

http://ip:port/OrderQuery/RMA/GetOrderRMAList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationFromSysNo | int | 否 | 卖家组织系统编码 |
| DataRangeSysNoList | array int | 否 | 数据范围编码列表（店铺树） |
| OrganizationToSysNo | int | 否 | 买家组织系统编码 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| PersonSysNo | int | 否 | 买家人员系统编码 |


> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RMASysNo | int | 是 | 退货单系统编码 |
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




#### AuditRecord说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AuditRecordSysNo | int | 是 | 系统编码 |
| AuditDate | string | 是 | 审核时间 |
| AuditRemark | string | 否 | 审核备注 |
| AuditPerson | object | 是 | 审核人实体（简） |























#获取已采购单列表（采购员）

##### _【功能说明】_ {#【功能说明】}

获取已采购单列表（采购员）


_**【应用场景】**_

获取已采购单列表（采购员）



_**【接口地址】**_
http://ip:port/OrderQuery/Order/GetBaidPurchaseOrderList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationFromSysNo | int | 是 | 采购员组织系统编码 |
| DataRangeSysNo | int | 否 | 采购员范围树编码（店铺树） |

> #### 应答_数据（数组）_ {#请求数据}


| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PurchaseOrderSysNo| int | 是 | 采购单流水编码 |
| SkuSysNo| int | 是 | SKU系统编码 |
| SkuName| string| 是 | SKU名称 |
| ProductGroupSysNo| int | 是 | 款系统编码 |
| ProductGroupName| int | 是 | 款名称 |
| OrganizationFromSysNo| int | 是 | 采购员组织|
| DataRangeSysNo| int | 是 | 采购员范围树编码（店铺树）|
| TotalAmount| decimal| 是 | 总金额 |
| UnitPrice| decimal| 是 | 单价|
| SkuFileThumbnailUrlList| array[string]| 是 | SKU缩略图|
| ProductFileThumbnailUrlList| array[string]| 是 | 款缩略图|




# 获取供应商记账单 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取供应商记账单

_**【应用场景】**_

获取供应商记账单

_**【接口地址】**_

[http://ip:port/OrganizationQuery/Supplier/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)SupplierBillList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SupplierSysNo | int | 是 | 供应商系统编码 |
| BillStartDate | string | 否 | 账单开始日期 |
| BillEndDate | string | 否 | 账单结束日期 |
| ProductGroupCodeList | array string | 否 | 款号列表 |
| IsGroupByProductGroup | int | 否 | 是否以款号汇总 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SupplierBillList | array object | 是 | 供应商记账单列表 |
| SupplierBillStatistics | object | 是 | 统计 |

#### SupplierBill说明_ _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SupplierBillSysNo | int | 是 | 系统编码 |
| BillDate | string | 是 | 账单日期 |
| ProductClassSysNo | int | 否 | 类别主键 |
| ProductGroupSysNo | int | 否 | 款系统编码 |
| ProductGroupCode | string | 否 | 款号 |
| SkuSysNo | int | 否 | 款SKU系统编码 |
| Count | int | 否 | 数量 |
| Amount | decimal（18，2） | 是 | 金额 |

#### SupplierBillStatistics说明_ _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TotalCount | int | 是 | 数量累计 |
| TotalAmount | decimal（18，2） | 是 | 金额累计 |




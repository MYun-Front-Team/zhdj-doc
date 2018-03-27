# 采购统计（采购员）

##### _【功能说明】_ {#【功能说明】}

采购统计（采购员）

_**【应用场景】**_

采购统计（采购员）

_**【接口地址】**_  
http://ip:port/OrderQuery/Order/GetPurchaseOrderTotal

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationFromSysNo | int | 是 | 采购员组织系统编码 |
| DataRangeSysNo | int | 是 | 采购员范围树编码（店铺树） |
| OrganizationToSysNo | int | 否 | 买家（商家）组织系统编码 |
| PersonSysNo | int | 否 | 买家（商家）人员系统编码 |
| OrderStartTime | string | 否 | 订单开始时间 |
| OrderEndTime | string | 否 | 订单结束时间 |
| PurchaseOrderType| int | 否 |（10） 已采购，（0）未采购 |
| KeyWord| string | 否 | 关键字 |



> #### 应答_数据（数组）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PurchaseOrderCount| int | 是 | 采购数量 |
| PurchaseOrderAmount| decimal | 是 | 采购数量金额 |





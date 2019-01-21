#获取蓝晶兑换订单列表

##### _【功能说明】_ {#【功能说明】}

获取蓝晶兑换订单列表

_**【应用场景】**_

获取蓝晶兑换订单列表

_**【接口地址】**_

http://ip:port/OrderQuery/LJOrder/GetLJChangeOrderList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| KeyWord| string| 否 | 关键字 |
| OrganizationFromSysNo | int | 否 | 卖家组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围树编码（店铺树） |
| OrganizationToSysNo | int |否 | 买家组织系统编码 |
| PersonSysNo | int | 否 | 买家人员系统编码 |
| DeliveryStatusList|array[int] | 否 |发货状态（10已发货，0待发货）|
| OrderStartTime | string | 否 | 开始时间（订单创建时间） |
| OrderEndTime | string | 否 | 结束时间（订单创建时间） |



> #### 返回数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Total| Total| 否 |统计信息 |
| Details| array[Detail]| 否 |订单列表信息 |

#### Total

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |



#### Detail

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 否 | 系统编码 |
| OrganizationFromSysNo | int | 是 | 卖家组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树编码（店铺树） |
| OrganizationToSysNo | int | 是 | 买家组织系统编码 |
| PersonSysNo | int | 是 | 买家人员系统编码 |
| DeliveryStatus| int | 是 | 发货状态（0待发货，10已发货） |
| DetailItems| array[DetailItem]| 是 | 订单详情|
| ReceiverName| string| 是 | 收货人 |
| ReceiverPhone| string| 是 | 收货人手机 |
| ReceiverAddress| string| 是 | 收货人地址 |
| PCDCode| string| 是 | 收货人省市区 |
| PCDDescription| string| 是 | 收货人省市区 |
| CreateTime| datetime| 是 | 创建时间 |
| TotalPointLJ| decimal | 否 | 总价|
| PersonName | string| 是 | 买家人员昵称 |
| CellPhoneNo| string| 是 | 买家人员手机 |
| TrackingCompanyCode| string| 是 | 快递公司编号 |
| TrackingCompanyName| string| 是 | 快递公司名称 |
| TrackingCompanySysNo| int| 是 | 快递公司系统编号 |
| TrackingNo| string| 是 | 快递单号 |


#### DetailItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo| int | 否 | 款系统编码 |
| SkuSysNo| int | 否 | SKU系统编码 |
| Quantity| int | 否 | 数量 |
| FloatPointPrice| decimal | 否 | 单价|
| ProductGroupName| string| 否 | 商品名称 |
| FileThumbnailUrlList| array string | 是 | 款缩略图 |



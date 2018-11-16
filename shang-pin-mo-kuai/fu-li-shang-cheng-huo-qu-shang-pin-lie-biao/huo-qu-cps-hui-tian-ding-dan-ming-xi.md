#获取CPS回填订单列表

##### _【功能说明】_ {#【功能说明】}

获取CPS回填订单列表

_**【应用场景】**_

获取CPS回填订单列表

_**【接口地址】**_

http://ip:port/OrderQuery/FLOrder/GetFLOrderBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 否 | 买家人员系统编码 |



> #### 返回数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderSysNo | int | 否 | 买家人员系统编码 |
| OrganizationFromSysNo | int | 是 | 卖家组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树编码（店铺树） |
| OrganizationToSysNo | int | 是 | 买家组织系统编码 |
| PersonSysNo | int | 是 | 买家人员系统编码 |
| OrderStatus| int | 是 | 订单状态（1待填订单号，2等待奖励，10已完成，11已关闭，12订单有误） |
| WaitCodeSecond| int| 否 | 待填订单号秒数|
| SourceOrderCode| string| 是 | 三方订单号|
| DetailItems| array[DetailItem]| 是 | 三方订单号|
| PersonName | string| 是 | 买家人员昵称 |
| CellPhoneNo| string| 是 | 买家人员手机 |
| FillSourceOrderCodeTime| datetime| 是 | 填三方订单号时间|
| CreateTime| datetime| 是 | 创建时间 |
| TotalPrice| decimal | 否 | 总价|
| TotalReward| decimal | 否 | 效果预估|



#### DetailItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo| int | 否 | 款系统编码 |
| SkuSysNo| int | 否 | SKU系统编码 |
| Quantity| int | 否 | 数量 |
| UnitPrice| decimal | 否 | 单价|
| RealPrice| decimal | 否 | 总价|
| Const| decimal | 否 | 成本价|
| ProductGroupName| string| 否 | 商品名称 |
| SourceCPSSysNo| int | 是 | 来源CPS系统编码 |
| SourceCPSName| string| 是 | 来源CPS名称 |
| SourceCPSCode| string| 是 | 来源CPSCode |
| FileThumbnailUrlList| array string | 是 | 款缩略图 |




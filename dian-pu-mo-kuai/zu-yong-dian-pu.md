# 租用店铺（摊位） {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

租用店铺（摊位）

_**【应用场景】**_

租用店铺（摊位）

注：1、判断摊位没有被租用过；

2、根据商家获取组织，绑定组织与摊位的租用关系；~~（如果没有默认店铺，则设置首个租用为默认）~~

3、填写租用表；

_**【接口地址】**_

[http://ip:port/ShopAction/Shop/L](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)easeShop

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ~~ShopSysNo~~ | ~~int~~ | ~~是~~ | ~~店铺系统编码~~ |
| BoothSysNo | int | 是 | 摊位系统编码 |
| SellerSysNo | int | 是 | 商家系统编码 |
| ShopRentFee | decimal\(18,2\) | 否 | 店铺实际租金（元/月） |
| ShopDepositFee | decimal\(18,2\) | 否 | 店铺实际押金 |
| RentStartDate | string | 否 | 租用开始日期 |
| RentEndDate | string | 否 | 租用结束日期 |
| Remark | string | 否 | 备注 |
| RentStatus | int | 是 | 租用状态：10租用，11解除 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




# 修改摊位 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改摊位

_**【应用场景】**_

修改摊位

_**【接口地址】**_

[http://ip:port/ShopAction/Booth/E](http://ip:port/OrganizationAction/Customer/AddCustomer)ditBooth

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BoothSysNo | int | 是 | 系统编码 |
| CategorySysNo | int | 否 | 主营类目主键 |
| BoothName | string | 否 | 摊位名称 |
| BoothNo | string | 否 | 摊位编号 |
| BoothArea | decimal（18，2） | 否 | 摊位面积（平方） |
| BoothPropertyFee | decimal（18，2） | 否 | 摊位物业费（元/年） |
| BoothDepositFee | decimal（18，2） | 否 | 摊位默认押金（元） |
| BoothRentFee | decimal（18，2） | 否 | 摊位默认租金（元/月） |
| BoothRentRemark | string | 否 | 摊位租用备注 |

#### _应答数据 _ {#应答数据-}




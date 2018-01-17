# 启动店铺开店状态 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

启动店铺开店状态

_**【应用场景】**_

启动店铺开店状态

注：1、从DataRangeSysNo、ShopSysNo、DeviceSysNo唯一定位到一个店铺Shop，标记店铺的OpenStatus；

都不传的话就取该组织的默认店铺；

2、记录操作人系统编码到“OpenPersonSysNo”；

3、开店的时候填写店铺与摊位的关系表；关店的时候删除该关系；

_**【接口地址】**_

[http://ip:port/ShopAction/Device/SetS](http://ip:port/OrganizationAction/Customer/AddCustomer)hopOpenStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围树结点（店铺树） |
| ShopSysNo | int | 否 | 店铺系统编码 |
| DeviceSysNo | int | 否 | 设备系统编码 |
| OpenStatus | int | 是 | 开店状态：10开，11关 |

#### _应答数据 _ {#应答数据-}




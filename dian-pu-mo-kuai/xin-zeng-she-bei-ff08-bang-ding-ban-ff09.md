# 新增设备（绑定版） {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增设备

_**【应用场景】**_

新增设备

~~注：新增设备并绑定到店铺中；~~

注：根据摊位编号找到摊位系统编码，如果摊位与设备已经绑定则直接返回结果；

_**【接口地址】**_

[http://ip:port/ShopAction/Device/AddD](http://ip:port/OrganizationAction/Customer/AddCustomer)eviceWithBanding

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ~~OrganizationSysNo~~ | ~~int~~ | ~~否~~ | ~~组织系统编码~~ |
| ~~DataRangeSysNo~~ | ~~int~~ | ~~否（二选一必填）~~ | ~~数据范围树枝叶编码（店铺树）~~ |
| ~~ShopSysNo~~ | ~~int~~ | ~~否（二选一必填）~~ | ~~店铺系统编码~~ |
| DeviceName | string | 是 | 设备名称 |
| DeviceNo | string | 否 | 设备编号 |
| BoothNo | string | 是 | 摊位编号 |

#### _应答数据 _ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceSysNo | int | 是 | 系统编码 |




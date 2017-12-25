# 新增设备 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增设备

_**【应用场景】**_

新增设备

注：记录所属关系表；

_**【接口地址】**_

[http://ip:port/ShopAction/Device/AddD](http://ip:port/OrganizationAction/Customer/AddCustomer)evice

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 否（可选配置） | 数据范围树枝叶编码（店铺树） |
| DeviceName | string | 是 | 设备名称 |
| DeviceNo | string | 否（可选配置） | 设备编号 |

#### _应答数据 _ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceSysNo | int | 是 | 系统编码 |




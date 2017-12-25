# 设置设备租用关系 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

设置设备租用关系

_**【应用场景】**_

设置设备租用关系

注：场景1：绑定租用：判断设备的DeviceStatus=0，才能租用，租用成功后设置=10，并记录租用关系表；

场景2：解除租用；删除租用关系，并设置DeviceStatus=0；

_**【接口地址】**_

[http://ip:port/ShopAction/Device/SetD](http://ip:port/OrganizationAction/Customer/AddCustomer)eviceStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 否（可选配置） | 数据范围树枝叶编码（店铺树） |
| DeviceSysNo | int | 是 | 设备系统编码 |
| DeviceStatus | int | 是 | 设备状态：0闲置，10使用 |

#### _应答数据 _ {#应答数据-}




# 添加待监视设备

##### _【功能说明】_ {#【功能说明】}

添加待监视设备

_**【应用场景】**_

添加待监视设备

_**【接口地址】**_

http://ip:port/UMAction/DeviceStatus/AddDeviceStatus


> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceName| string| 是 | 设备名称 |
| DeviceCode| string| 是 | 设备唯一编码 |
| DataRangeSysNo| int| 是 | 数据范围编码 |

> #### _应答数据（Propertys数组）_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| | int | 是 | 系统编码 |




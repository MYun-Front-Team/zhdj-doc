# 获取监视设备详情

##### _【功能说明】_ {#【功能说明】}

获取监视设备详情

_**【应用场景】**_

获取监视设备详情

_**【接口地址】**_

http://ip:port/UMQuery/DeviceStatus/GetDeviceStatusBySysNo
> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceSysNo | int | 是 | 系统编码 |




> #### _应答数据（Propertys数组）_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceSysNo | int | 是 | 系统编码 |
| DeviceName| string| 是 | 设备名称 |
| DeviceCode| string| 是 | 设备唯一编码 |
| HeartBeat| string| 是 | 最后心跳时间|
| HeartStatus| int | 是 |状态（0初始，10正常，9警告，11下线） |







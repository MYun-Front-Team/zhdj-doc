# 编辑监视设备

##### _【功能说明】_ {#【功能说明】}

编辑监视设备

_**【应用场景】**_

编辑监视设备

_**【接口地址】**_

http://ip:port/UMAction/DeviceStatus/EditDeviceStatus


> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceSysNo | int | 是 | 系统编码 |
| DeviceName| string| 是 | 设备名称 |
| DeviceCode| string| 是 | 设备唯一编码 |
| HeartBeat| string| 是 | 最后心跳时间|
| HeartStatus| int | 是 |状态（0初始，10正常，9警告，11下线） |




# 新增设备

_**【接口地址】**_

http://ip:port/VDAction/Detect/AddDevice

> #### _请求数据_ 

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| dsSysNo | int | 是 | 检测站id |
| DeviceName | string | 是 | 设备名称 |
| StartDate | datetime | 是 | 设备有效期起 |
| EndDate | datetime | 是 | 设备有效期止 |

> #### _应答数据 _

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 设备id |




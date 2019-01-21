# 获取设备消息发送状态列表

_**【接口地址】**_

http://ip:port/MessageQuery/Message/GetMessagePublishStatusList
> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MsgId | int | 否 | 消息编码 |

> #### _应答数据 _

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MsgId | int | 是 | 消息编码 |
| DeviceSysNo | int | 是 | 设备编码 |
| DeviceName | string | 是 | 设备别名 |
| DeviceCode | string | 是 | 设备编号 |
| PublishStatus | int | 是 | 1待发送，2发送中，10发送成功，11发送失败 |



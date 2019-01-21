# 设置发送结果 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/MessageAction/Message/SetPublishResult](http://ip:port/MessageAction/Message/EditMaterial)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MsgId | int | 是 | 消息编码 |
| DeviceCode | string | 是 | 设备编号 |
| status | int | 是 | 0发送中，1成功，2失败 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |





# 获取未发送消息

_**【接口地址】**_

http://ip:port/MessageQuery/Message/GetMsgUnsendByDeviceCode
> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceCode | string | 是 | 设备编号 |

> #### _应答数据 _

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MsgId | int | 是 | 消息编码 |
| MsgType | int | 是 | 1群发，2朋友圈 |
| Content | string | 是 | 文本内容 |
| FileUrlList | array[string] | 是 | 资源内容列表 |




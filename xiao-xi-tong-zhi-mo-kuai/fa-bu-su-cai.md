# 发布素材 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/MessageAction/Message/PublishMaterial](http://ip:port/MessageAction/Message/EditMaterial)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MaterialSysNo | int | 是 | 素材编码 |
| RecordType | int | 是 | 1群发，2朋友圈 |
| DeviceList | array\[int\] | 否 | 设备列表 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 消息编码 |





# 发布素材 

_**【接口地址】**_

http://ip:port/MessageAction/Message/PublishMaterial

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MaterialSysNo | int | 是 | 素材编码 |
| RecordType | int | 是 | 1群发，2朋友圈 |
| DeviceList | array\[object\] | 否 | 设备列表 |

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceId | int | 是 | 设备id |
| Friends | array[string] | 是 | 好友列表 |


> #### _应答数据 _ 

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 消息编码 |





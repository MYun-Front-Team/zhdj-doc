# 获取发布记录列表

_**【接口地址】**_

http://ip:port/MessageQuery/Message/GetPublishRecordList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 否 | 人员编码 |
| IsShowFriends | int | 否 | 1显示好友的发布记录 |

> #### _应答数据 _

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecordSysNo | int | 是 | 发布记录编码 |
| RecordType | int | 是 | 1群发，2朋友圈 |
| PersonSysNo | int | 是 | 人员编码 |
| PersonName | string | 是 | 昵称 |
| CellPhoneNo | string | 是 | 手机 |
| AvatarUrl | string | 是 | 头像 |
| Text | string | 是 | 文本内容 |
| UrlList | array\[string\] | 是 | 资源内容列表 |
| DeviceList | array\[object\] | 是 | 设备列表 |
| CreateTime | datetime | 是 | 创建时间 |
| PublishTime | datetime | 是 | 发布时间 |
| RecordStatus | int | 是 | 1待发送，2进行中，10已成功，11已失败，12已取消 |

#### _设备_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceSysNo | int | 是 | 设备id |
| DeviceName | string | 是 | 别名 |
| DeviceCode | string | 是 | 设备编号 |
|  |  |  |  |




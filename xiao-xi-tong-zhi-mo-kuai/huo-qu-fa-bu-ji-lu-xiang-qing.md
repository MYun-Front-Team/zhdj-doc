# 获取发布记录详情 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/MessageQuery/Message/GetPublishRecordBySysNo](http://ip:port/MessageQuery/Message/GetMaterialList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PublishRecordSysNo | int | 否 | 发布记录编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

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

#### _设备_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceSysNo | int | 是 | 设备id |
| DeviceName | string | 是 | 别名 |
| DeviceCode | string | 是 | 设备编号 |
|  |  |  |  |




# 获取素材列表 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/MessageQuery/Message/GetMaterialList](http://ip:port/MessageQuery/Message/GetMaterialList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 否 | 人员编码 |
| IsShowFriends | int | 否 | 1显示好友素材 |
| GroupSysNoList | array int | 否 | 分组id列表 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MaterialSysNo | int | 是 | 素材编码 |
| PersonSysNo | int | 是 | 人员编码 |
| PersonName | string | 是 | 昵称 |
| CellPhoneNo | string | 是 | 手机 |
| AvatarUrl | string | 是 | 头像 |
| Text | string | 是 | 文本内容 |
| UrlList | array\[string\] | 是 | 资源内容列表 |
| CreateTime | datetime | 是 | 创建时间 |




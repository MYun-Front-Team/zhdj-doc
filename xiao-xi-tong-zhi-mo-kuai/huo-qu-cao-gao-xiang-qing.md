# 获取草稿详情

_**【接口地址】**_

http://ip:port/MessageQuery/Message/GetDraftBySysNo

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DraftSysNo | int | 是 | 草稿编码 |


> #### _应答数据 _

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DraftSysNo | int | 是 | 草稿编码 |
| PersonSysNo | int | 是 | 人员编码 |
| PersonName | string | 是 | 昵称 |
| CellPhoneNo | string | 是 | 手机 |
| AvatarUrl | string | 是 | 头像 |
| Text | string | 是 | 文本内容 |
| UrlList | array\[string\] | 是 | 资源内容列表 |
| CreateTime | datetime | 是 | 创建时间 |
| GroupSysNo | int | 是 | 分组id |
| GroupName | string | 是 | 分组名称 |



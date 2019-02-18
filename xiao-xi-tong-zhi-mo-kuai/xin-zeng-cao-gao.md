# 新增草稿

_**【接口地址】**_

http://ip:port/MessageAction/Message/AddDraft

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员编码 |
| GroupSysNo | int | 否 | 分组id |
| Text | string | 否 | 文本 |
| UrlList | array[string] | 否 | 资源内容列表 |

> #### _应答数据 _

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MaterialSysNo | int | 是 | 草稿编码 |



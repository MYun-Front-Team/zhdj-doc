# 新增分组 

_**【接口地址】**_

http://ip:port/MessageAction/Message/AddGroup

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员编码 |
| GroupName | string | 是 | 分组名称 |
| GroupType | int | 否 | 0素材分组，1草稿分组 |

> #### _应答数据 _ 

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 是 | 分组编码 |




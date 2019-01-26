# 获取分组详情 

_**【接口地址】**_

http://ip:port/MessageQuery/Message/GetGroupBySysNo

默认分组不可用该接口

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 是 | 分组编码 |

> #### _应答数据 _ 

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 是 | 分组编码 |
| GroupName | string | 是 | 分组名称 |
| PersonSysNo | int | 是 | 人员编码 |
| Count | int | 是 | 数量 |
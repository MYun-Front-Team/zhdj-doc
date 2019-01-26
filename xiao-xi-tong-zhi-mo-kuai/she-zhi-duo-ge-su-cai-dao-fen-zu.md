# 设置多个素材到分组

_**【接口地址】**_

http://ip:port/MessageAction/Message/SetMaterialGroup

默认分组不可用该接口

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 是 | 分组编码 |
| MaterialSysNoList | array int | 是 | 素材编码列表 |

> #### _应答数据 _ 

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
# 发消息 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

发消息

_**【应用场景】**_

发消息

注：判断群成员是否在线，不在线则需要推送到设备。

_**【接口地址】**_

[http://ip:port/ChatAction/Chat/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)endGroupMsg

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 是 | 群系统编码 |
| MsgID | string | 否 | 消息ID |
| MsgType | string | 是 | 消息内容形式（端自定义） |
| MsgContent | string | 是 | 消息内容（端自定义） |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MsgSysNo | int | 是 | 群消息系统编码 |




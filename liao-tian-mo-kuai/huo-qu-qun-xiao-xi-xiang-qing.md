# 获取群消息详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取群消息详情

_**【应用场景】**_

获取群消息详情

注：需记录浏览人在该条消息中的浏览次数。

_**【接口地址】**_

[http://ip:port/ChatQuery/Chat/G](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etMsgBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MsgSysNo | int | 是 | 群消息系统编码 |
|  |  |  |  |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MsgSysNo | int | 是 | 消息系统编码 |
| MsgID | string | 否 | 消息ID |
| Person | object | 是 | 发送人成员实体（见基础模块登录） |
| MsgType | int | 是 | 消息内容形式（端自定义） |
| MsgContent | string | 是 | 消息内容（端自定义） |




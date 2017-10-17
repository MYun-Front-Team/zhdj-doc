# 获取群消息详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取群消息详情

_**【应用场景】**_

获取群消息详情

注：自动设置该群消息全部已读。

_**【接口地址】**_

[http://ip:port/ChatQuery/Chat/G](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etGroupMsgList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupSysNo | int | 是 | 群系统编码 |
| MsgStartTime | string | 否 | 消息开始时间 |
| MsgEndTime | string | 否 | 消息结束时间 |

> #### _应答数据 （Msg）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MsgSysNo | int | 是 | 消息系统编码 |
| MsgID | string | 否 | 消息ID |
| Person | object | 是 | 发送人成员实体（见基础模块登录） |
| MsgType | int | 是 | 消息内容形式（端自定义） |
| MsgContent | string | 是 | 消息内容（端自定义） |




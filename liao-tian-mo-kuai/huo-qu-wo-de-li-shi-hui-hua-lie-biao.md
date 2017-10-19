# 获取我的历史会话列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取我的历史会话列表

_**【应用场景】**_

获取我的历史会话列表

_**【接口地址】**_

[http://ip:port/ChatQuery/Chat/G](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etMyHistoryGroupMsgList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MsgStartTime | string | 否 | 消息开始时间 |
| MsgEndTime | string | 否 | 消息结束时间 |
| IsStrangerMsg | int | 否 | 是否陌生人消息（设置1则返回单聊+陌生人的会话列表） |
| Limit | object | 否 | 限制条件 |

> #### _应答数据 （数据）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupBase | object | 是 | 群基础字段实体 |
| GroupStatistic | object | 是 | 计算字段实体 |
| Msg | object | 是 | 最后一条消息实体 |
| Person | object | 是 | 好友实体（单聊时返回） |




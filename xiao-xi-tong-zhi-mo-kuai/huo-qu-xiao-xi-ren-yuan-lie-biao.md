# 获取消息人员列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取消息人员列表

_**【应用场景】**_

获取消息人员列表

_**【接口地址】**_

[http://ip:port/MessageQuery/Message/G](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etMessagePersonList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MessageSysNo | int | 否 | 消息系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MessagePersonSysNo | int | 是 | 消息人员系统编码 |
| Person | object | 是 | 人员实体 |
| ReadStatus | int | 是 | 状态：0已发，1已达，10已读 |
| SendTime | string | 否 | 发送时间 |
| ReceiverTime | string | 否 | 接收时间 |
| ReadTime | string | 否 | 阅读时间 |




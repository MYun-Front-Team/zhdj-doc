# 修改消息 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改消息

_**【应用场景】**_

修改消息

注：只有草稿和撤销状态，可以修改；

_**【接口地址】**_

[http://ip:port/MessageAction/Message/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditMessage

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MessageSysNo | int | 是 | 消息系统编码 |
| MessageTitle | string | 是 | 标题 |
| MessageContent | string | 是 | 内容 |
| MessageType | int | 是 | 消息类型：0短信，1微信模板消息，2APP |
| IsPublic | int | 是 | 是否公开：0否，1是 |
| PickRuleTemplateList | array object | 是 | 选人规则（见选人模块说明） |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




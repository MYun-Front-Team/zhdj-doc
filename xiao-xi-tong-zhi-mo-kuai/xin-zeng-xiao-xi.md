# 新增消息 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增消息

_**【应用场景】**_

新增消息

注：新增后为草稿状态，消息人员表不需要填充；

_**【接口地址】**_

[http://ip:port/MessageAction/Message/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddMessage

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | array int | 是 | 数据范围枝叶编码列表（必须在不同的树中的枝叶） |
| ModuleSysNo | int | 是 | 模块编码（枚举） |
| ModuleSourceType | int | 是 | 模块类型（枚举） |
| ModuleSourceClass | int | 否 | 模块分类编码（枚举） |
| MessageTitle | string | 是 | 标题 |
| MessageContent | string | 是 | 内容 |
| MessageType | int | 是 | 消息类型：0短信，1微信模板消息，2APP |
| IsPublic | int | 是 | 是否公开：0否，1是 |
| PickRuleTemplateList | array object | 是 | 选人规则（见选人模块说明） |
| SponsorName | string | 否 | 主办方 |
| CoSponsorName | string | 否 | 协办方 |
| FilePathList | array string | 否 | 文件或图片Path列表（第一张为首图） |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MessageSysNo | int | 是 | 消息系统编码 |




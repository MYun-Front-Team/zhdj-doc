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
| IsForce| int | 是 | 是否不管状态强行编辑 |
| MessageTitle | string | 是 | 标题 |
| MessageContent | string | 是 | 内容 |
| MessageType | int | 是 | 消息类型：0短信，1微信模板消息，2APP |
| IsPublic | int | 是 | 是否公开：0否，1是 |
| PickRuleTemplateList | array object | 是 | 选人规则（见选人模块说明） |
| SponsorName | string | 否 | 主办方 |
| CoSponsorName | string | 否 | 协办方 |
| FilePathList | array string | 否 | 文件或图片Path列表（第一张为首图） |
| OrganizationSysNo | int | 否 | 组织系统编码 |
| SponsorDataRangeSysNo| int| 否 | 主办方ID |
| MessageTypeList|array[int] | 否 | 消息类型：0短信，1微信模板消息，2APP |
| ObjectFileList| array File| 否（可选配置） | 附件 |
| MessageObjectList| array File| 否（可选配置） | 消息附属对象|

> #### MessageObject

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 是 | 来源系统编码 |
| OrganizationSysNo | int | 是 | 商品组织系统编码 |


#### File说明 {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FileTitle| string| 是 | 文件名称 |
| FilePath| string| 是 | 文件地址 |





> #### _应答数据 _ {#应答数据-（巡河记录数组）}




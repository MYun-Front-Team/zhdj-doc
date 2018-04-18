# 消息通知模块-字段说明 {#新增河流}

> #### MessageBase基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MessageSysNo | int | 是 | 消息系统编码 |
| ModuleSysNo | int | 是 | 模块编码（枚举） |
| ModuleSourceType | int | 否 | 模块类型（枚举） |
| ModuleSourceClass | int | 否 | 模块分类编码（枚举） |
| ModuleSourceSysNo | int | 否 | 模块来源系统编码 |
| MessageStatus | int | 是 | 消息状态（0草稿，10已发送， 11撤销） |
| MessageTitle | string | 是 | 标题 |
| MessageContent | string | 是 | 内容 |
| MessageType | int | 是 | 消息类型：0短信，1微信模板消息，2APP |
| IsPublic | int | 是 | 是否公开：0否，1是 |
| SponsorName | string | 否 | 主办方 |
| CoSponsorName | string | 否 | 协办方 |
| PublishTime | string | 否 | 发布时间 |
| PublishPerson | object | 否 | 发布人实体 |
| RemoveTime | string | 否 | 撤下人时间 |
| RemovePerson | object | 否 | 撤下人实体 |
| FilePathList | array string | 否 | 文件或图片Path列表（第一张为首图） |
| FileUrlList | array string | 否 | 文件或图片URL列表（第一张为首图） |


> #### MessageStatistic统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SendCount | int | 否 | 发送数量 |
| ReceiverCount | int | 否 | 接收数量 |
| ReadedCount | int | 否 | 阅读数量 |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### Query查询字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| MessageSysNo | int | 否 | 消息系统编码 |
| ModuleSysNo | int | 否 | 模块编码（枚举） |
| ModuleSourceType | int | 否 | 模块类型（枚举） |
| ModuleSourceClass | int | 否 | 模块分类编码（枚举） |
| ModuleSourceSysNo | int | 否 | 模块来源系统编码 |
| MessageStatusList | Array\[int\] | 否 | 消息状态（0草稿，10已发送， 11撤销） |
| MessageTitle | string | 否 | 标题 |
| MessageType | int | 否 | 消息类型：0短信，1微信模板消息，2APP |
| IsPublic | int | 否 | 是否公开：0否，1是 |
|  |  |  |  |
| IsOwner | int | 否 | 是否显示自己的消息（被圈到的全部消息） |
| IsCreator | int | 否 | 是否显示自己创建的消息 |

> #### Limit限制字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowSendCount | int | 否 | 是否显示发送数量 |
| IsShowReceiverCount | int | 否 | 是否显示接收数量 |
| IsShowReadedCount | int | 否 | 是否显示阅读数量 |
| IsShowFileUrlList  | int | 否 | 是否显示主图 |

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |





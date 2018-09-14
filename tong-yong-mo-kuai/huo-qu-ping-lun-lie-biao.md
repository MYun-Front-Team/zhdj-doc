# 获取评论列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取评论列表

_**【应用场景】**_

获取评论列表

_**【接口地址】**_

http://ip:port/UMQuery/Comment/GetCommentList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 组织系统编码 |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 否 | 来源系统编码 |
| ShowStatusList | array int | 否 | 显示状态：0不显示，1显示 |
| IsMyFootPrint | int | 否 | 是否显示自己的：0否，1是（不传查全部，传值需通过UserSysNo匹配Person） |
| Limit | object | 否 | 限制条件 |
| KewWord | string | 否 | 关键字（内容） |
| AuditStatus | int | 否 | 回复状态：0否，1是 |
| AverageStartScore | decimal\(18,2\) | 否 | 开始分数 |
| AverageEndScore | decimal\(18,2\) | 否 | 结束分数 |
| SemesterSysNo | int | 否 | 学期系统编码 |


> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CommentSysNo | int | 是 | 系统编码 |
| CommentSource | int | 是 | 评论来源：1系统，2官网，3IOS，4-安卓，5-HTML5 |
| CommentContent | string | 是 | 评论内容 |
| CommentUrlList | array string | 否 | 图片URL路径列表 |
| Person | object | 是 | 评论人员实体（简版） |
| IsAnonymous | int | 是 | 是否匿名：0否，1是 |
| Propertys | array object | 否 | 评论明细列表（见通用-属性） |
| ModuleRelation | object | 否 | 模块关联实体 |
| AuditRecord | object | 否 | 回复实体（同审核） |
| AuditStatus | int | 否 | 回复状态：0否，1是 |
| SemesterSysNo | int | 否 | 学期系统编码 |



#### Limit说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowModuleRelation | int | 否 | 是否显示模块信息 |
| IsShowAuditRecord | int | 否 | 是否显示回复记录 |




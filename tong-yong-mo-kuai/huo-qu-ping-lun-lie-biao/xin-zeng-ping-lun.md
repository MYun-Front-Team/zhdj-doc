# 新增评论 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增评论

_**【应用场景】**_

新增评论

注：CommentSource=1表示系统自动评论；

_**【接口地址】**_

[http://ip:port/UMAction/Comment/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddComment

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 否 | 来源系统编码 |
| ModuleRelations| array[ModuleRelation]| 是 | 附属模块|
| CommentSource | int | 是 | 评论来源：1系统，2官网，3IOS，4-安卓，5-HTML5 |
| CommentContent | string | 是 | 评论内容 |
| IsAnonymous | int | 是 | 是否匿名：0否，1是 |
| CommentPathList | array string | 否 | 图片Path路径列表 |
| Propertys | array object | 是 | 评论明细列表（见通用-属性） |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CommentSysNo | int | 是 | 系统编码 |

#### ModuleRelation

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 关联模块编码 |
| ModuleSourceType | int | 否 | 关联模块类型 |
| ModuleSourceClass | int | 否 | 关联模块分类 |
| ModuleSourceSysNo | int | 是 | 关联模块来源编码 |








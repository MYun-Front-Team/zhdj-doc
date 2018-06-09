# 多个模块一起评论

##### _【功能说明】_ {#【功能说明】}

多个模块一起评论

_**【应用场景】**_

多个模块一起评论



_**【接口地址】**_

http://ip:port/UMAction/Comment/AddGroupComment

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CommentSource | int | 是 | 评论来源：1系统，2官网，3IOS，4-安卓，5-HTML5 |
| CommentContent | string | 是 | 评论内容 |
| IsAnonymous | int | 是 | 是否匿名：0否，1是 |
| CommentPathList | array string | 否 | 图片Path路径列表 |
| Propertys | array object | 是 | 评论明细列表（见通用-属性） |

#### ModuleRelation

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 否 | 来源系统编码 |





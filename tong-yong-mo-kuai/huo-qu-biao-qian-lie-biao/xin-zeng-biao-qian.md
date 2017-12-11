# 新增标签 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增标签

_**【应用场景】**_

新增标签

_**【接口地址】**_

[http://ip:port/UMAction/Tag/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddTag

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| ~~ModuleSysNo~~ | ~~int~~ | ~~是~~ | ~~模块编码~~ |
| ~~ModuleSourceType~~ | ~~int~~ | ~~否~~ | ~~来源类型~~ |
| ~~ModuleSourceClass~~ | ~~int~~ | ~~否~~ | ~~来源分类~~ |
| ~~ModuleSourceSysNo~~ | ~~int~~ | ~~否~~ | ~~来源系统编码~~ |
| TagType | int | 是 | 标签类型（枚举） |
| TagName | string | 是 | 标签名称 |
| TagPathList | array string | 否 | 标签图片path列表 |
| IconColor | string | 否 | 标签底色 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TagSysNo | int | 是 | 系统编码 |




# 获取标签列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取标签列表

_**【应用场景】**_

获取标签列表

注：标签枚举：1商品标签，2收货地址标签，3品牌标签，4订单标签，5工单标签，6网格员，7人员，8客户标签

_**【接口地址】**_

[http://ip:port/UMQuery/Tag/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)TagList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| ~~ModuleSysNo~~ | ~~int~~ | ~~是~~ | ~~模块编码~~ |
| ~~ModuleSourceType~~ | ~~int~~ | ~~否~~ | ~~来源类型~~ |
| ~~ModuleSourceClass~~ | ~~int~~ | ~~否~~ | ~~来源分类~~ |
| ~~ModuleSourceSysNo~~ | ~~int~~ | ~~否~~ | ~~来源系统编码~~ |
| TagType | int | 否 | 标签类型（枚举） |
| TagTypeList | array[int] | 否 | 标签类型（枚举） |
| IsHiddenList | array int | 否 | 是否对前台隐藏（1隐藏，0可见） |
| ShowTypeList | array[int] | 否 | 展示方式 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TagSysNo | int | 是 | 系统编码 |
| TagName | string | 是 | 标签名称 |
| TagUrlList | array string | 否 | 标签URL列表 |
| PosterUrlList | array string | 否 | 海报URL列表 |
| IconColor | string | 否 | 标签底色 |
| IsHidden | int | 否 | 是否对前台隐藏（1隐藏，0可见） |
| SortNo | int | 是 | 排序 |
| IsSystem | int | 是 | 是否系统标签 |
| ShowTypeList | array[int] | 否 | 展示方式 |


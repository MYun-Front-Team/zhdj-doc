# 获取品牌列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取品牌列表

_**【应用场景】**_

获取品牌列表

_**【接口地址】**_

[http://ip:port/UMQuery/Brand/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)BrandList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| ~~ModuleSysNo~~ | ~~int~~ | ~~是~~ | ~~模块编码~~ |
| ~~ModuleSourceType~~ | ~~int~~ | ~~否~~ | ~~来源类型~~ |
| ~~ModuleSourceClass~~ | ~~int~~ | ~~否~~ | ~~来源分类~~ |
| ~~ModuleSourceSysNo~~ | ~~int~~ | ~~否~~ | ~~来源系统编码~~ |
| IsEnable | int | 否 | 是否启用（影响前台展示） |
| IsEnableInBack | int | 否 | 是否后台启用 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BrandSysNo | int | 是 | 系统编码 |
| BrandName | string | 是 | 品牌名称 |
| IsEnable | int | 是 | 是否启用（影响前台展示） |
| IsEnableInBack | int | 是 | 是否后台启用 |
| BrandUrlList | array string | 否 | 图片Url路径列表 |




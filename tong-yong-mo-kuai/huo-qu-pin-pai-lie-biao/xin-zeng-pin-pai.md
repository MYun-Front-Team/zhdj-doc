# 新增品牌 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增品牌

_**【应用场景】**_

新增品牌

_**【接口地址】**_

[http://ip:port/UMAction/Brand/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddBrand

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 否 | 来源系统编码 |
| BrandName | string | 是 | 品牌名称 |
| IsEnable | int | 否 | 是否启用（影响前台展示） |
| IsEnableInBack | int | 否 | 是否后台启用 |
| BrandPathList | array string | 否 | 图片path路径列表 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BrandSysNo | int | 是 | 系统编码 |




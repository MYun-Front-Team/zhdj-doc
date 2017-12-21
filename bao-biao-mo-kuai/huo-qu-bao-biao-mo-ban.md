# 获取报表模板 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取报表模板

_**【应用场景】**_

获取报表模板

_**【接口地址】**_

[http://ip:port/BIQuery/BI/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)BITemplate

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceType | int | 是 | 来源类型 |
| ModuleSourceClass | int | 是 | 来源分类 |
| ModuleSourceSysNo | int | 是 | 来源系统编码 |
| PageSysNo | int | 是 | 页编码 |
| PageHtmlStyle | int | 是 | 页类型（同一个页，可能存在不同的样式） |
| ~~PageRequestData~~ | ~~object~~ | ~~否~~ | ~~请求参数（具体报表具体分析）~~ |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PageHtmlSysNo | int | 是 | 系统编码 |
| PageHtmlStyle | int | 是 | 页类型 |
| PageHtmlName | string | 是 | 页标题 |
| PageHtml | string | 是 | HTML |
| Remark | string | 否 | 备注 |
| ~~PageResponseData~~ | ~~object~~ | ~~是~~ | ~~数据实体（具体报表具体分析）~~ |




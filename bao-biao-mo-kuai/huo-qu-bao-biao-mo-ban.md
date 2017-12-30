# 获取报表模板 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取报表模板

_**【应用场景】**_

获取报表模板

注：如果通过Module没有搜索到个性化的模板，那么使用通用的模板；

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

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PageHtmlSysNo | int | 是 | 系统编码 |
| PageHtmlStyle | string | 是 | HTML扩展 |
| PageHtmlName | string | 是 | 页标题 |
| PageHtml | string | 是 | HTML |
| Remark | string | 否 | 备注 |




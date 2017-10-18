# 获取选人规则 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取选人规则

_**【应用场景】**_

获取选人规则

_**【接口地址】**_

[http://ip:port/PickQuery/Pick/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)PickRule

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块编码（枚举） |
| ModuleSourceSysNo | int | 是 | 模块来源系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PickRuleTemplateList | array object | 是 | 选人规则（见模块说明） |




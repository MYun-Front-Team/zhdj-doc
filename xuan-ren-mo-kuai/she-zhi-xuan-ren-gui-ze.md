# ~~设置选人规则~~ {#获取河长巡河记录}

##### ~~_【功能说明】_~~ {#【功能说明】}

~~设置选人规则~~

~~_**【应用场景】**_~~

~~设置选人规则~~

~~_**【接口地址】**_~~

[~~http://ip:port/PickAction/Pick/S~~](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)~~etPickRule~~

> #### ~~_请求数据_~~ {#请求数据}

| ~~变量名~~ | ~~类型~~ | ~~是否必须~~ | ~~描述~~ |
| :--- | :--- | :--- | :--- |
| ~~ModuleSysNo~~ | ~~int~~ | ~~是~~ | ~~模块编码（枚举）~~ |
| ~~ModuleSourceType~~ | ~~int~~ | ~~否~~ | ~~模块类型（枚举）~~ |
| ~~ModuleSourceClass~~ | ~~int~~ | ~~否~~ | ~~模块分类编码（枚举）~~ |
| ~~ModuleSourceSysNo~~ | ~~int~~ | ~~是~~ | ~~模块来源系统编码~~ |
| ~~Remark~~ | ~~string~~ | ~~否~~ | ~~备注~~ |
| ~~PickRuleTemplateList~~ | ~~array object~~ | ~~是~~ | ~~选人规则（见模块说明）~~ |

> #### ~~_应答数据 _~~ {#应答数据-（巡河记录数组）}

| ~~变量名~~ | ~~类型~~ | ~~是否必须~~ | ~~描述~~ |
| :--- | :--- | :--- | :--- |
| ~~PickRuleSysNo~~ | ~~int~~ | ~~是~~ | ~~选人规则系统编码~~ |




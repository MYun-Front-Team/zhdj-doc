# 新增分润规则 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增分润规则

_**【应用场景】**_

新增分润规则

注：ProfitRuleGroupSysNo=0则取默认值；

分润比率总和不能超过100%；

_**【接口地址】**_

[http://ip:port/WalletAction/ProfitRule/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddProfitRule

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitRuleGroupSysNo | int | 否 | 分润规则组系统编码 |
| ModuleRelation | object | 否 | 来源模块关联 |
| OperateType | int | 否 | 来源操作类型（枚举） |
| ProfitRuleName | string | 是 | 分润角色分类名称 |
| Remark | string | 否 | 备注 |
| ProfitRuleDetailList | array object | 否 | 分润规则明细列表 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitRuleSysNo | int | 是 | 系统编码 |

####  {#应答数据-（巡河记录数组）}




# 修改分润规则 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改分润规则

_**【应用场景】**_

修改分润规则

_**【接口地址】**_

[http://ip:port/WalletAction/ProfitRule/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditProfitRule

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitRuleSysNo | int | 否 | 系统编码 |
| OperateType | int | 否 | 来源操作类型（枚举） |
| ProfitRuleName | string | 是 | 分润角色分类名称 |
| Remark | string | 否 | 备注 |
| ProfitRuleDetailList | array object | 否 | 分润规则明细列表 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




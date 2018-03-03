# 分润规则管理-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitRuleSysNo | int | 是 | 分润规则系统编码 |
| ProfitRuleGroupSysNo | int | 是 | 分润规则组系统编码 |
| ModuleRelation | object | 否 | 来源模块关联 |
| OperateType | int | 否 | 来源操作类型（枚举） |
| ProfitRuleName | string | 是 | 分润角色分类名称 |
| Remark | string | 否 | 备注 |
| ProfitRuleGroup | object | 否 | 分润规则组 |
| ProfitRuleDetailList | array object | 否 | 分润规则明细列表 |

> #### ProfitRuleDetail说明_ _ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitRuleDetailSysNo | int | 是 | 分润规则明细系统编码 |
| ProfitRoleSysNo | int | 是 | 分润角色系统编码 |
| ProfitRole | object | 是 | 分润角色 |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| OrganizationBossPerson | object | 是 | 组织默认联系人 |
| ProfitRate | decimal（18，4） | 是 | 分润比率 |
| Remark | string | 否 | 备注 |
| ProfitRole | object | 否 | 分润角色 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| UsedProfitRate | decimal（18，4） | 否 | 该规则已使用分润比率 |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| KeyWord | string | 否 | 关键字搜索（名称） |
| ProfitRuleGroupSysNo | int | 是 | 分润规则组系统编码 |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowProfitRuleGroup | int | 否 | 是否显示分润规则组 |
| IsShowProfitRuleDetailList | int | 否 | 是否显示分润规则明细 |
| IsShowProfitRole | int | 否 | 是否显示分润角色 |
| IsShowUsedProfitRate | int | 否 | 是否显示已使用分润比率 |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}




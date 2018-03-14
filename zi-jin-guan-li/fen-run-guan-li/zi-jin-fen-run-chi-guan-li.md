# 资金分润池管理-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitPoolSysNo | int | 是 | 分润池系统编码 |
| OrganizationSysNo | int | 是 | 付款方组织系统编码 |
| ModuleRelation | object | 否 | 模块关联 |
| AgentType | int | 否 | 冗余代理商类型 |
| AgentPCDCode | string | 否 | 冗余代理省市区Code |
| AgentPCDDescription | string | 否 | 冗余代理省市区描述 |
| ProfitPoolSourceType | int | 是 | 分润资金来源：0线上，1线下 |
| ProfitPoolType | int | 是 | 资金类型：0代理费，1广告费，2会员费，3交易佣金 |
| ProfitPoolAmount | decimal（18，2） | 是 | 分润资金 |
| ProfitPoolStatus | int | 是 | 分润池状态：0待分润，10已分润，11已作废 |
| ProfitRuleSysNo | int | 否 | 分润规则系统编码 |
| Remark | string | 否 | 备注 |
| Organization | object | 否 | 组织 |
| ProfitPoolDetailList | array object | 否 | 分润明细列表 |

> #### ProfitPoolDetail说明_ _ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitPoolDetailSysNo | int | 是 | 分润资金池明细系统编码 |
| ProfitRoleSysNo | int | 是 | 分润角色系统编码 |
| OrganizationSysNo | int | 是 | 组织系统编码（与分润角色关联） |
| OrganizationName | string | 否 | 组织名称 |
| ProfitRate | decimal（18，4） | 是 | 分润比率 |
| ProfitAmount | decimal（18，2） | 是 | 分润到金额 |
| Remark | string | 否 | 备注 |
| ProfitRole | object | 否 | 分润角色 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitTotalAmount | decimal（18，2） | 否 | 已分润总金额 |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProfitPoolStatusList | array int | 否 | 分润池状态：0待分润，10已分润，11已作废 |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowOrganization | int | 否 | 是否显示组织 |
| IsShowProfitPoolDetailList | int | 否 | 是否显示分润明细列表 |
| IsShowProfitTotalAmount | int | 否 | 是否显示已分润总金额 |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}




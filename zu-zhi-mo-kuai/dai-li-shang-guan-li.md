# 代理商模块-字段说明 {#新增河流}

> #### AgentBase基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| AgentSysNo | int | 是 | 代理商系统编码 |
| AgentType | int | 是 | 代理商类型（代理枚举） |
| AgentClassSysNo | int | 否 | 代理商类别系统编码（类目树） |
| AgentClassName | string | 否 | 代理商类别名称 |
| AgentLevelSysNo | int | 否 | 代理商等级系统编码 |
| AuditStatus | int | 是 | 审核状态：0待审核，10审核通过，11审核失败 |
| AuditRecord | object | 否 | 审核记录实体 |
| AgentStatus | int | 是 | 代理商状态：10有效，11无效 |
| AgentName | string | 是 | 代理商名称 |
| AgentShortName | string | 是 | 代理商简称 |
| AgentTel | string | 否 | 代理商联系电话 |
| AgentDesc | string | 否 | 代理商描述 |
| AgentMaster | string | 否 | 代理商负责人 |
| AgentPost | string | 否 | 代理商负责人岗位 |
| AgentIDCard | string | 否 | 代理商负责人身份证 |
| AgentGender | int | 否 | 代理商负责人性别：1男，2女 |
| AgentPerson | string | 否 | 代理商联系人 |
| AgentPersonPhone | string | 否 | 代理商联系人电话 |
| AgentPersonPost | string | 否 | 代理商联系人岗位 |
| PCDCode | string | 否 | 省市区代码 |
| PCDDescription | string | 否 | 省市区描述 |
| ContractAddress | string | 否 | 联系地址 |
| Longitude | decimal\(18,2\) | 否 | 经度 |
| Latitude | decimal\(18,2\) | 否 | 纬度 |
| Remark | string | 否 | 备注 |
| IDCardPathList | array string | 否 | 身份证Path路径列表 |
| IDCardUrlList | array string | 否 | 身份证Url路径列表 |
| AgentLogoPathList | array string | 否 | 代理商Logo路径列表 |
| AgentLogoUrlList | array string | 否 | 代理商Logo的URL列表 |
| AgentPCDCode | string | 是 | 代理区域Code |
| AgentPCDDescription | string | 是 | 代理区域描述 |
| AgentBossPerson | object | 否 | 代理商创始人实体（默认联系人） |

> #### AgentStatistic统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Wallet | object | 否 | 钱包实体（资金说明） |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### Query查询字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| AgentSysNo | int | 否 | 代理商系统编码 |
| AuditStatusList | Array\[int\] | 否 | 审核状态 |
| AgentStatusList | Array\[int\] | 否 | 代理商状态 |
| KeyWord | string | 否 | 关键字（名称/负责人/联系人/电话） |

> #### Limit限制字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IDCardUrlList | int | 否 | 是否显示身份证列表 |
| IsShowWallet | int | 否 | 是否显示钱包 |
| IsShowAgentBossPerson | int | 否 | 是否显示代理商创始人 |

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |


#### AuditRecord说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AuditRecordSysNo | int | 是 | 系统编码 |
| AuditDate | string | 是 | 审核时间 |
| AuditRemark | string | 否 | 审核备注 |
| AuditResult | int | 是 | 审核结果：10审核通过，11审核失败 |
| AuditPerson | object | 是 | 审核人实体（简） |




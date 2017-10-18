# 选人模块-字段说明 {#新增河流}

> #### PickBase基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PickSysNo | int | 是 | 系统编码 |
| ModuleSysNo | int | 是 | 模块编码（枚举） |
| ModuleSourceType | int | 否 | 模块类型（枚举） |
| ModuleSourceClass | int | 否 | 模块分类系统编码（类别树） |
| ModuleSourceSysNo | int | 是 | 模块来源系统编码 |
| Remark | string | 否 | 备注 |
| PickRuleTemplateList | array object | 是 | 选人规则 |

#### RuleTemplate说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeGradeType | int | 是 | 等级类型：1省，2市，3区，4街道/县，5社区/村，51支部 |
| DataRangeGradeName | string | 是 | 等级名称 |
| Propertys | array object | 否 | 属性列表（含值） |
| DataRangeSysNoList | array int | 否 | 数据范围系统编码列表 |
| RulePersonList | array int | 否 | 人员列表 |

#### RulePerson说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Person | object | 是 | 人员实体（简版） |
| ExcludeStatus | int | 是 | 状态： 0新添，1排除 |

> #### PickStatistic统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### Query查询字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### Limit限制字段 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |


####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |





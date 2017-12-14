# 客户模块-字段说明 {#新增河流}

> #### CustomerBase基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CustomerSysNo | int | 是 | 客户系统编码 |
| CustomerLevelSysNo | int | 否 | 客户等级系统编码 |
| CustomerStatus | int | 是 | 状态：0待发展，10正常，11终止 |
| CustomerName | string | 是 | 客户名称 |
| CustomerShortName | string | 是 | 简称 |
| CustomerTel | string | 否 | 客户联系电话 |
| CustomerDesc | string | 否 | 客户描述 |
| CustomerMaster | string | 否 | 客户负责人 |
| CustomerPost | string | 否 | 客户负责人岗位 |
| CustomerPerson | string | 否 | 客户联系人 |
| CustomerPersonPhone | string | 否 | 客户联系人电话 |
| CustomerPersonPost | string | 否 | 客户联系人岗位 |
| ContractAddress | string | 否 | 联系地址 |
| Longitude | decimal\(18,2\) | 否 | 经度 |
| Latitude | decimal\(18,2\) | 否 | 纬度 |
| CustomerLogoPathList | array string | 否 | 客户Logo的路径列表 |
| CustomerLogoUrlList | array string | 否 | 客户Logo的Url列表 |

> #### CustomerStatistic统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### Query查询字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| CustomerSysNo | int | 否 | 客户系统编码 |
| CustomerStatusList | Array\[int\] | 否 | 状态：0待发展，10正常，11终止 |
| KeyWord | string | 否 | 关键字（名称/负责人/联系人/电话） |

> #### Limit限制字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |





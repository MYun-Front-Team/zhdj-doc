# 供应商模块-字段说明 {#新增河流}

> #### SupplierBase基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SupplierSysNo | int | 是 | 供应商系统编码 |
| SupplierLevelSysNo | int | 否 | 供应商等级系统编码 |
| SupplierStatus | int | 是 | 状态：0待发展，10正常，11终止 |
| SupplierName | string | 是 | 供应商名称 |
| SupplierShortName | string | 是 | 简称 |
| SupplierTel | string | 否 | 供应商联系电话 |
| SupplierDesc | string | 否 | 供应商描述 |
| SupplierMaster | string | 否 | 供应商负责人 |
| SupplierPost | string | 否 | 供应商负责人岗位 |
| SupplierPerson | string | 否 | 供应商联系人 |
| SupplierPersonPhone | string | 否 | 供应商联系人电话 |
| SupplierPersonPost | string | 否 | 供应商联系人岗位 |
| ContractAddress | string | 否 | 联系地址 |
| Longitude | decimal\(18,2\) | 否 | 经度 |
| Latitude | decimal\(18,2\) | 否 | 纬度 |
| SupplierLogoPathList | array string | 否 | 供应商Logo的路径列表 |
| SupplierLogoUrlList | array string | 否 | 供应商Logo的URL列表 |

> #### SupplierStatistic统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### Query查询字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| SupplierSysNo | int | 否 | 供应商系统编码 |
| SupplierStatusList | Array\[int\] | 否 | 状态：0待发展，10正常，11终止 |
| KeyWord | string | 否 | 关键字（名称/负责人/联系人/电话） |

> #### Limit限制字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |





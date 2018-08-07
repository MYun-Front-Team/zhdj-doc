# 服务商模块-字段说明 {#新增河流}

> #### ServicerBase基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ServicerSysNo | int | 是 | 服务商系统编码 |
| ServicerType | int | 是 | 服务商类型（行业树） |
| ServicerClassSysNo | int | 否 | 服务商类别系统编码（类目树） |
| ServicerLevelSysNo | int | 否 | 服务商等级系统编码 |
| ServicerStatus | int | 是 | 状态：0待发展，10正常，11终止 |
| ServicerName | string | 是 | 服务商名称 |
| ServicerShortName | string | 是 | 简称 |
| ServicerTel | string | 否 | 服务商联系电话 |
| ServicerDesc | string | 否 | 服务商描述 |
| ServicerMaster | string | 否 | 服务商负责人 |
| ServicerPost | string | 否 | 服务商负责人岗位 |
| ServicerPerson | string | 否 | 服务商联系人 |
| ServicerPersonPhone | string | 否 | 服务商联系人电话 |
| ServicerPersonPost | string | 否 | 服务商联系人岗位 |
| ContractAddress | string | 否 | 联系地址 |
| Longitude | decimal\(18,2\) | 否 | 经度 |
| Latitude | decimal\(18,2\) | 否 | 纬度 |
| ServicerLogoPathList | array string | 否 | 服务商Logo的路径列表 |
| ServicerLogoUrlList | array string | 否 | 服务商Logo的Url列表 |
| Remar1| string | 否（可选配置） | 备注1|
| Remar2| string | 否（可选配置） | 备注2|
| Remar3| string | 否（可选配置） | 备注3|





> #### ServicerStatistic统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### Query查询字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| ServicerTypeList | Array\[int\] | 否 | 服务商类型（行业树） |
| ServicerSysNo | int | 否 | 供应商系统编码 |
| ServicerStatusList | Array\[int\] | 否 | 状态：0待发展，10正常，11终止 |
| KeyWord | string | 否 | 关键字（名称/负责人/联系人/电话） |
| ServicerNameFirstLetter | string | 否 | 服务商名称首字母 |

> #### Limit限制字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |





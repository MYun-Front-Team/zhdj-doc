# 商家模块-字段说明 {#新增河流}

> #### SellerBase基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SellerSysNo | int | 是 | 商家系统编码 |
| SellerLevelSysNo | int | 否 | 商家等级系统编码 |
| SellerStatus | int | 是 | 状态：0待发展，10正常，11终止 |
| SellerName | string | 是 | 商家名称 |
| SellerShortName | string | 是 | 简称 |
| SellerTel | string | 否 | 商家联系电话 |
| SellerDesc | string | 否 | 商家描述 |
| SellerMaster | string | 否 | 商家负责人 |
| SellerPost | string | 否 | 客户负责人岗位 |
| SellerPerson | string | 否 | 客户联系人 |
| SellerPersonPhone | string | 否 | 客户联系人电话 |
| SellerPersonPost | string | 否 | 客户联系人岗位 |
| ContractAddress | string | 否 | 联系地址 |
| Longitude | decimal\(18,2\) | 否 | 经度 |
| Latitude | decimal\(18,2\) | 否 | 纬度 |

> #### SellerStatistic统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### Query查询字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| SellerSysNo | int | 否 | 客户系统编码 |
| SellerStatusList | Array\[int\] | 否 | 状态：0待发展，10正常，11终止 |
| KeyWord | string | 否 | 关键字（名称/负责人/联系人/电话） |

> #### Limit限制字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |





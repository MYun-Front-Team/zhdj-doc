# 组织模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 是 | 组织所属数据范围树枝叶编码 |
| OrganizationType | int | 是 | 类型（枚举） |
| OrganizationClassSysNo | int | 否 | 类别系统编码（分类树） |
| OrganizationName | string | 是 | 组织名称 |
| OrganizationShortName | string | 否 | 组织简称 |
| OrganizationTel | string | 否 | 组织联系电话 |
| OrganizationDesc | string | 否 | 组织描述 |
| OrganizationMaster | string | 否 | 组织负责人 |
| OrganizationPost | string | 否 | 组织负责人岗位 |
| OrganizationPerson | string | 否 | 组织联系人 |
| OrganizationPersonPhone | string | 否 | 组织联系人电话 |
| OrganizationPersonPost | string | 否 | 组织联系人岗位 |
| ContractAddress | string | 否 | 联系地址 |
| Longitude | decimal（18，10） | 否 | 经度 |
| Latitude | decimal（18，10） | 否 | 纬度 |
| OrganizationLogoPathList | array string | 否 | 组织Logo的路径列表 |
| OrganizationLogoUrlList | array string | 否 | 组织Logo的Url列表 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Wallet | object | 是 | 钱包实体（资金说明） |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称） |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowWallet | int | 否 | 是否显示钱包 |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}

| 枚举值 | 模块说明 | 模块类型 | 模块类型分类 | 页面说明 |
| :--- | :--- | :--- | :--- | :--- |
| 1700101 | 组织模块 |  |  | 新增页 |
| 1700102 |  |  |  | 修改页 |
| 1700103 |  |  |  | 详情页 |
| 1700104 |  |  |  | 列表页 |




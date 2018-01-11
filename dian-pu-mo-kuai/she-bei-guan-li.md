# 设备管理-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树枝叶编码（店铺树） |
| DeviceSysNo | int | 是 | 设备系统编码 |
| DeviceName | string | 是 | 设备名称 |
| DeviceNo | string | 否 | 设备编号 |
| DeviceStatus | int | 是 | 设备状态：0闲置，10使用 |
|  |  |  |  |
| RentOrganization | object | 否 | 租用组织 |
| RentShop | object | 否 | 租用店铺 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationFromSysNo | int | 否 | 所有者组织系统编码 |
| DataRangeSysNoList | int | 否 | 数据范围树枝叶编码列表（店铺树） |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称） |
| OrganizationToSysNo | int | 否 | 租用方组织系统编码 |
| DeviceStatusList | array int | 否 | 设备状态：0闲置，10使用 |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowRentOrganization | int | 否 | 是否显示租用组织 |
| IsShowRentShop | int | 否 | 是否显示租用店铺 |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}




# 房间管理-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RoomSysNo | int | 是 | 系统编码 |
| HouseSysNo | int | 是 | 房屋系统编码 |
| RoomNo | string | 否 | 房间编号 |
| RoomName | string | 是 | 房间名称 |
| RoomArea | decimal\(18,2\) | 否 | 房间面积 |
| RoomOrientation | string | 否 | 房间朝向 |
| RoomPurpose | int | 否 | 房间用途：0自用，1出租 |
| RoomTenantNum | int | 否 | 承租户数量 |
| RoomPermitNum | int | 否 | 办证数量 |
| Propertys | array object | 否 | 房间属性列表 |
| TenantList | array object | 否 | 租户列表 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TenantCount | int | 否 | 租户数量 |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HouseSysNo | int | 否 | 房屋系统编码 |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowPropertys | int | 否 | 是否显示房间属性列表 |
| IsShowTenantList | int | 否 | 是否显示租户列表 |
| IsShowTenantCount | int | 否 | 是否显示租户数量 |

#### Tenant说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Resident | object | 是 | 居民实体 |
| IsTenant | int | 是 | 是否租户 |
| IsLive | int | 是 | 是否居住在该房间 |




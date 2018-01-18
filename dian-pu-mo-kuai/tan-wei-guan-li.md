# 摊位管理-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 所有者组织系统编码 |
| BoothSysNo | int | 是 | 摊位系统编码 |
| CategorySysNo | int | 是 | 主营类目主键 |
| CategoryName | string | 是 | 主营类目名称 |
| BoothName | string | 是 | 摊位名称 |
| BoothNo | string | 否 | 摊位编号 |
| BoothStatus | int | 是 | 摊位状态：0闲置，10使用 |
| BoothArea | decimal（18，2） | 是 | 摊位面积（平方） |
| BoothPropertyFee | decimal（18，2） | 否 | 摊位物业费（元/年） |
| BoothDepositFee | decimal（18，2） | 否 | 摊位默认押金（元） |
| BoothRentFee | decimal（18，2） | 否 | 摊位默认租金（元/月） |
| BoothRentRemark | string | 否 | 摊位租用备注 |
| SellerRent | object | 否 | 当前商家租用信息（见租用列表说明） |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DeviceCount | int | 否 | 设备数量 |
| SellerCount | int | 否 | 商家数量 |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 所有者组织系统编码 |
| CategorySysNoList | array int | 否 | 主营类目主键 |
| KeyWord | string | 否 | 关键字搜索（名称/编号） |
| BoothStatusList | array int | 否 | 状态：0闲置，10使用 |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowDeviceCount | int | 否 | 是否显示设备数量 |
| IsShowSellerCount | int | 否 | 是否显示商家数量 |
| IsShowSellerRent | int | 否 | 是否显示当前商家租用信息 |

####  {#应答数据-（巡河记录数组）}




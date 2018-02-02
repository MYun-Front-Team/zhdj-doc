# 网格管理-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GridSysNo | int | 是 | 系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树枝叶编码 |
| GridName | string | 是 | 网格名称 |
| GridRange | string | 否 | 网格范围 |
| GridMaster | string | 否 | 负责人 |
| GridManList | array object | 否 | 网格员列表 |
| FatherDataRange | array object | 否 | 上级数据范围列表 |
| GridMasterTel | string | 否 | 负责人电话 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GridManCount | int | 否 | 网格员数量 |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| GridSysNo | int | 否 | 网格系统编码 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称） |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowGridManList | int | 否 | 是否显示网格员列表 |
| IsShowFatherDataRange | int | 否 | 是否显示父级列表（值N代表父级级别） |
| IsShowGridManCount | int | 否 | 是否显示网格员数量 |

####  {#应答数据-（巡河记录数组）}




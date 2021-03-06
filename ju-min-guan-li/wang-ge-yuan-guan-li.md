# 网格员管理-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GridManSysNo | int | 是 | 系统编码 |
| GridManPerson | object | 是 | 人员（简版） |
| GridList | array object | 否 | 网格列表（简） |
| TagList | array object | 否 | 标签列表 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HouseCount | int | 否 | 房屋总数量 |
| HouseExCount | int | 否 | 房屋异常数量 |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| GridSysNo | int | 否 | 网格系统编码 |
| GridManSysNo | int | 否 | 网格员系统编码 |
| PersonSysNo | int | 否 | 人员系统编码 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称） |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowGridList | int | 否 | 是否显示网格列表 |
| IsShowTagList | int | 否 | 是否显示标签列表 |
| IsShowHouseCount | int | 否 | 是否显示房屋总数量 |
| IsShowHouseExCount | int | 否 | 是否显示房屋异常数量 |




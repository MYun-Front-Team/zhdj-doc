# 楼层管理

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ParkFloorSysNo | int | 是 | 楼层编码 |
| ParkSysNo | int | 是 | 园区编码 |
| BuildingSysNo | int | 是 | 楼宇编码 |
| ParkFloorType | int | 是 |楼层类型|
| ParkFloorClassSysNo | int | 否 | 楼层分类（枚举） |
| ParkFloorName | string | 否 | 楼层名称 |
| ParkFloorArea| decimal | 否 | 楼层面积|
| Remark | string | 否 | 楼层备注 |
| FilePathList | array string | 否 |照片 |
| FileUrlList | array string | 否 |照片 |


> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### 功能按钮字段 {#请求数据}

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 组织系统编码 |
| DataRangeSysNoList |array int | 否 | 数据范围树枝叶编码列表 |
| KeyWord | string | 否 | 关键字|
| BuildingSysNo | int | 是 | 楼宇系统编码 |
| ParkSysNo | int | 是 | 园区编码 |


> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |






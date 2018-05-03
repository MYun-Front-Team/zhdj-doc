# 楼宇管理-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BuildingSysNo | int | 是 | 楼宇系统编码 |
| ParkSysNo | int | 否 | 园区编码 |
| ParkName | string | 否 | 园区名称|
| BuildingType | int | 否|楼宇类型|
| BuildingClassSysNo | int | 否 | 楼宇分类（枚举） |
| BuildingName | string | 否 | 楼宇名称 |
| BuildingAddress | string | 否 | 地址 |
| BuildingPerson| string | 否 |联系人|
| BuildingPersonPhone| string | 否 |联系电话|
| Remark| string | 否 |备注|
| TotalArea| decimal | 否 |用地面积|
| BuildingArea| decimal | 否 |总建筑面积|
| BusinessArea| decimal | 否 |商务办公面积|
| ParkingLotArea| decimal | 否 |停车场面积|
| ParkingLotCount| int | 否 |机动车泊位数|
| ChargeForProperty | decimal| 否 |物业费|




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
| ParkSysNo | int | 是 | 园区系统编码 |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |






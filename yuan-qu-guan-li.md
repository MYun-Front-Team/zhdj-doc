# 园区管理-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ParkSysNo | int | 是 | 园区系统编码 |
| ParkType | int | 是 | 园区类型|
| ParkClassSysNo | int | 否 | 园区分类（枚举） |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树枝叶编码 |
| PCDCode | string | 否 | 省市区 代码 |
| PCDDescription | string | 否 | 省市区 名称 |
| ParkNumber | string | 否 | 园区编号|
| ParkName | string | 否 | 园区名称|
| ParkAddress | string | 否 | 园区地址|
| ParkArea | decimal| 否 | 园区面积|
| ChargeForWater| decimal| 否 |水费单价|
| ChargeForProperty | decimal| 否 |物业费|
| ChargeForElectric | decimal| 否 |电费单|
| ParkPerson| string | 否 |联系人|
| ParkPersonPhone| string | 否 |联系电话|
| Remark| string | 否 |备注|
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
| PCDCode | string | 否 | 省市区 代码 |
| PCDDescription | string | 否 | 省市区 名称 |
| KeyWord | string | 否 | 关键字|


> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |






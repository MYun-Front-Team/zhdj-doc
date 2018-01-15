# 获取业务属性列表 {#获取河长详情}

##### _【功能说明】_ {#【功能说明】}

获取业务属性列表

_**【应用场景】**_

获取业务属性列表

_**【接口地址】**_

[http://ip:port/UMQuery/Property/GetObjectPropert](http://ip:port/HMQuery/RiverMaster/GetRiverMasterByRiverMasterSysNo)ys

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块编码（枚举） |
| ModuleSourceType | int | 否 | 模块类型（枚举） |
| ModuleSourceClass | int | 否 | 模块类型分类编码（分类） |

> #### _应答数据（Propertys数组）_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PropertySysNo | int | 是 | 属性系统编码 |
| PropertyType | int | 是 | 属性适应类型 |
| PropertyName | string | 是 | 属性名 |
| IsAllowNull | int | 是 | 是否允许空 |
| IsOptional | int | 是 | 属性值类型：0文本，1单休，2多选，3关联 |
| PropertyValues | array object | 否 | 属性值列表 |

#### PropertyValue说明 {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PropertyValueSysNo | int | 是 | 属性值系统编码 |
| PropertySysNo | int | 是 | 属性系统编码 |
| PropertyValue | string | 是 | 属性值 |
| PropertyUrl | string | 否 | 属性图片 |
| SelectedCount | int | 否 | 选中数量 |
| SelectedPercent | decimal（18，4） | 否 | 选中比例 |




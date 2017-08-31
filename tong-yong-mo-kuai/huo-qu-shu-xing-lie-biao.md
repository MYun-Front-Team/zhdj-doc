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
| SourceType | int | 是 | 来源类型 |
| SourceSysNo | int | 是 | 来源编码 |
| IsShowPropertyValues | int | 否 | 是否显示默认属性值列表 |

> #### _应答数据（Propertys数组）_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PropertySysNo | int | 是 | 属性系统编码 |
| PropertyName | string | 是 | 属性名 |
| IsAllowNull | int | 是 | 是否允许空 |
| IsOptional | int | 是 | 属性值类型：0文本，1单休，2多选 |
| PropertyValues | array object | 否 | 属性值列表 |

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PropertyValueSysNo | int | 是 | 属性值系统编码 |
| PropertySysNo | int | 是 | 属性系统编码 |
| PropertyValue | string | 是 | 属性值 |
| SortNo | int | 否 | 排序 |




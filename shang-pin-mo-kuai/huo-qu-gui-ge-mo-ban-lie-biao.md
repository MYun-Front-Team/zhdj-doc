# 获取规格模板列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取规格模板列表

_**【应用场景】**_

获取规格模板列表

注：获取组织下的规格模板参数说明：OrganizationSysNo和SpecGroupType=1；

获取某个店铺的规格模块则DataRangeSysNo&gt;0；

_**【接口地址】**_

[http://ip:port/ProductQuery/Spec/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)SpecTemplateList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围结点系统编码 |
| SpecGroupType | int | 是 | 规格组类型：1商品规格组，2商品冗余规格组 |

> #### _应答数据 （SpecGroup）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SpecGroupSysNo | int | 是 | 规格组系统编码 |
| SpecGroupName | string | 是 | 规格组名称 |
| SpecList | array object | 是 | 规格列表 |

#### Spec {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SpecSysNo | int | 是 | 规格系统编码 |
| SpecName | string | 是 | 规格名称 |
| SpecValueList | array object | 是 | 规格值列表 |

#### SpecValue {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SpecValueSysNo | int | 是 | 规格值系统编码 |
| SpecName | string | 是 | 规格名称 |
| SpecValue | string | 是 | 规格值 |
| SpecValueOtherName | string | 否 | 规格值别名 |
| IsCustomized | int | 是 | 是否可定制：0否，1是 |
| IsChecked | int | 否 | 是否选中：0否，1是 |
| IconColor | string | 否 | 色号 |
| SpecValueFee | decimal\(18,2\) | 否 | 费用 |
| SpecValueUrlList | array string | 否 | 图片 |




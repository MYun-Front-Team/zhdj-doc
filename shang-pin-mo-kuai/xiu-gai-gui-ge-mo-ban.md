# 修改规格模板 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改规格模板

_**【应用场景】**_

修改规格模板

_**【接口地址】**_

[http://ip:port/ProductAction/Spec/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditSpecTemplate

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Spec | object | 是 | 商品规格实体 |

> #### _应答数据 （Spec）_ {#应答数据-（巡河记录数组）}

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
| SpecValue | string | 是 | 规格值 |
| ~~SpecValueOtherName~~ | ~~string~~ | ~~否~~ | ~~规格值别名~~ |
| IsCustomized | int | 是 | 是否可定制：0否，1是 |
| ~~IsChecked~~ | ~~int~~ | ~~否~~ | ~~是否选中：0否，1是~~ |
| IconColor | string | 否 | 色号 |
| SpecValueFee | decimal\(18,2\) | 否 | 费用 |
| SpecValuePathList | array string | 否 | 图片 |




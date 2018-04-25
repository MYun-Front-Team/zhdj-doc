# 新增资金分润 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

添加园区

_**【应用场景】**_

添加园区

_**【接口地址】**_

http://ip:port/ParkAction/IndustryPark/AddPark

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ParkType | int | 是 | 园区类型|
| ParkClassSysNo | int | 否 | 园区分类（枚举） |
| OrganizationSysNo | int | 是 | 平台组织系统编码 |
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
> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ParkSysNo | int | 是 | 园区系统编码 |



# 获取用户列表 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/WTQuery/Water/GetUserList](http://ip:port/EqmQuery/Equipment/GetEquipmentList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 否 | 登录人id |
| OrganizationTypeList | array int | 否 | 17031小区负责人，17032小区物业，17033水务局 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织编码 |
| PersonSysNo | int | 是 | 人员编码 |
| OrganizationType | int | 是 | 组织类型 |
| PersonName | string | 是 | 姓名 |
| CellPhoneNo | string | 是 | 手机号 |
| LastLoginDate | datetime | 是 | 最近登录时间 |
| Password | string | 是 | 密码 |
| UserGender | int | 是 | 1男，2女 |
| IsEnable | int | 是 | 1启用，2禁用 |
| HouseEstateList | array HouseEstate | 是 | 负责小区列表 |

HouseEstate

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HouseEstateSysNo | int | 是 | 小区id |
| HouseEstateName | string | 是 | 小区名称 |
| PCDCode | string | 是 | 省市区编码 |
| PCDDescription | string | 是 | 省市区名称 |
| Location | string | 是 | 具体地址 |




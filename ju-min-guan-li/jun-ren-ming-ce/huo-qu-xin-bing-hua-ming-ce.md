# 获取军人名册列表

##### _【功能说明】_ {#【功能说明】}

获取军人名册列表

_**【应用场景】**_

获取军人名册列表

_**【接口地址】**_

[http://ip:port/ResidentQuery/Resident/GetResidentSoldierYearList](http://ip:port/ResidentQuery/Resident/GetResidentSoldierYearList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | array int | 否 | 数据范围树编码列表 |
| SoldierYearType | int | 否 | 名册类型（1新兵花名册2现役军人名册3退伍军人名册） |
| Year | int | 是 | 年度 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| Name | string | 否 | 姓名 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ResidentSoldierYearSysNo | int | 是 | 系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树编码 |
| DataRanges | array\[DataRange\] | 是 | 省市区街道 |
| Year | int | 是 | 年度 |
| Sex | int | 是 | 性别：1男，2女 |
| Name | string | 是 | 姓名 |
| Nation | string | 是 | 民族 |
| OriginType | int | 是 | 籍贯性质（1城镇，2乡村） |
| BirthDay | Datetime | 是 | 生日 |
| Education | int | 是 | 学历：0未知,1小学,2初中,3中转,4高中,5专科,6本科,7硕士,8博士，10高校新生 |
| PoliticalType | int | 是 | 政治面貌（1党员2团员3群众） |
| Remark | string | 是 | 去向 |
| ArmyType | int | 是 | 军种1陆军2海军3空军4火箭军5战略支援部队6武警 |
| InArmyDate | Datetime | 是 | 入伍时间 |
| OutArmyDate | Datetime | 是 | 退伍时间 |
| MilitaryRank | string | 是 | 军衔 |
| Lat | decimal | 是 | 纬度 |
| Lon | decimal | 是 | 经度 |
| Address | string | 是 | 详细地址 |




# 获取干部和党支部详情

##### _【功能说明】_ {#【功能说明】}

获取干部和党支部详情

_**【应用场景】**_

获取干部和党支部详情

_**【接口地址】**_

[http://ip:port/ResidentAction/Resident/AddResidentSoldierYear](http://ip:port/ResidentAction/Resident/AddResidentSoldierYear)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SoldierYearType | int | 是 | 名册类型（1新兵花名册2现役军人名册3退伍军人） |
| DataRangeSysNo | int | 是 | 数据范围树编码 |
| Year | int | 是 | 年度 |
| Sex | int | 是 | 性别：1男，2女 |
| Name | string | 是 | 姓名 |
| Nation | string | 是 | 民族 |
| OriginType | int | 是 | 籍贯性质（1城镇，2乡村） |
| BirthDay | Datetime | 是 | 生日 |
| Education | int | 是 | 学历：0未知,1小学,2初中,3中转,4高中,5专科,6本科,7硕士,8博士 |
| PoliticalType | int | 是 | 政治面貌（1党员2团员3群众） |
| Remark | string | 否 | 去向 |
| ArmyType | int | 否 | 军种1陆军2海军3空军4火箭军5战略支援部队6武警 |
| InArmyDate | Datetime | 否 | 入伍时间 |
| OutArmyDate | Datetime | 否 | 退伍时间 |
| MilitaryRank | string | 否 | 军衔 |
| Address | string | 否 | 详细地址 |
| FullAddress | string | 否 | 定位地址 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ResidentSoldierYearSysNo | int | 是 | 系统编码 |




# 修改 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改

_**【应用场景】**_

修改

_**【接口地址】**_

[http://ip:port/RecruitAction/Position/E](http://ip:port/HMAction/River/AddRiver)ditPosition

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionSysNo | int | 是 | 职位系统编码 |
| PositionName | Nvarchar\(50\) | 是 | 职位名称（冗余） |
| PositionType | int | 否 | 工作类型:0不限,1全职,2兼职 |
| SexType | int | 否 | 性别要求：0不限,1男，2女 |
| RecruitCount | int | 否 | 招聘人数 |
| ExperienceRequirements | int | 否 | 经验要求：0不限,1一年内，2一到三年，3三到五年，4五到十年，5十年以上 |
| Remark | Nvarchar\(max\) | 否 | 备注 |
| PositionPathList | array string | 否 | 工作地Path文件列表 |
| PositionSalaryList | array object | 否 | 客户可见岗位薪资列表 |
| PositionAgeList | array object | 否 | 岗位年龄列表 |
| PositionWorkDayList | array object | 否 | 工作日期列表 |
| PositionWorkTimeList | array object | 否 | 工作时间列表 |
| TagSysNoList | array int | 否（可选配置） | 标签列表 |
| TagClassList | array object | 否 | 福利标签列表（说明见通用） |
| CustomerPositionName| Nvarchar\(50\) | 否 | 客户自定义职位名称 |
| PositionDayAreaList | array object | 否 | 工作日期列表（日期） |
| PlatPositionSalaryList | array object | 否 | 平台岗位薪资列表 |
|IsHot| int | 否 |是否热门岗位|
|HotStartTime| datetime | 否 |热门开始|
|HotEndTime| int | 否 |热门结束|
|IsBonus| int | 否 |是否返佣|
|BonusAmount| decimal | 否 |返佣金额|


> #### 工作日期PositionWorkDay（兼职有效）

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionWorkDaySysNo | int | 否 | 工作日期系统编码（0新增，非0编辑）|
| DayOfWeek | int | 是 | （0周日，1周一，2周二……6周六，7做一休一 8做二休二） |

> #### 工作时间点PositionWorkTime（兼职有效）

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionWorkTimeSysNo | int | 否 | 工作时间点系统编码（0新增，非0编辑）|
| StartTime | datetime | 是 |开始时间 |
| EndTime | datetime | 是 |结算时间 |
| WorkTimeType| int| 是 |0其他 1早班 2中班 3晚班（班次） |

> #### 工作日期（时间）PositionDayArea（兼职有效）

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionDayAreaSysNo | int | 是 | 工作日期系统编码|
| StartTime | datetime | 是 |开始时间 |
| EndTime | datetime | 是 |结束时间 |

> #### TagClass

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TagClassSysNo | int | 否 | 福利编码（分类）  |
| TagClassName| string| 是 |福利名称  |


> #### PositionSalary 薪资 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SalaryType | int | 是 | 薪资类型：1月，2天，3时 |
| SalaryMax | Decimal\(18,2\) | 是 | 最大值 |
| SalaryMin | Decimal\(18,2\) | 是 | 最小值 |
| Remark | Nvarchar\(max\) | 否 | 备注 |











#### _应答数据_ {#应答数据-}




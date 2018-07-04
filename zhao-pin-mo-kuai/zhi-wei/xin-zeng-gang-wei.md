# 新增 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增

_**【应用场景】**_

新增

_**【接口地址】**_

[http://ip:port/RecruitAction/Position/Add](http://ip:port/HMAction/River/AddRiver)Position

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 否 | 所属数据范围树 |
| ShopSysNo | int | 否 | 店铺系统编码 |
| PositionClassSysNo | int | 是 | 职位类型编码（分类） |
| PositionName | Nvarchar\(50\) | 是 | 职位名称（冗余） |
| PositionType | int | 否 | 工作类型:0不限,1全职,2兼职 |
| SexType | int | 否 | 性别要求：0不限,1男，2女 |
| RecruitCount | int | 否 | 招聘人数 |
| ExperienceRequirements | int | 否 | 经验要求：0不限,1一年内，2一到三年，3三到五年，4五到十年，5十年以上 |
| Remark | Nvarchar\(max\) | 否 | 备注 |
| PositionPathList | array string | 否 | 工作地Path文件列表 |
| PositionSalaryList | array object | 否 | 岗位薪资列表 |
| PositionAgeList | array object | 否 | 岗位年龄列表 |
| PositionWorkDayList | array object | 否 | 工作日期列表 |
| PositionWorkTimeList | array object | 否 | 工作时间列表 |
| TagClassList | array object | 否 | 福利标签列表（说明见通用） |
| CustomerPositionName| Nvarchar\(50\) | 否 | 客户自定义职位名称 |
| PositionDayAreaList | array object | 否 | 工作日期列表（日期） |











> #### 工作日期PositionWorkDay（兼职有效）

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DayOfWeek | int | 是 | （0周日，1周一，2周二……6周六） |

> #### 工作时间点PositionWorkTime（兼职有效）

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StartTime | datetime | 是 |开始时间 |
| EndTime | datetime | 是 |结算时间 |

> #### 工作日期（时间）PositionDayArea（兼职有效）

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StartTime | datetime | 是 |开始时间 |
| EndTime | datetime | 是 |结束时间 |





> #### TagClass

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TagClassSysNo | int | 否 | 福利编码（分类）  |
| TagClassName| string| 是 |福利名称  |




#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionSysNo | int | 是 | 系统编码 |

####  {#应答数据-}




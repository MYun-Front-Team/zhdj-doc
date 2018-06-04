# 职位模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionSysNo | int | 是 | 职位系统编码 |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 否 | 所属数据范围树 |
| ShopSysNo | int | 否 | 店铺系统编码 |
| PositionClassSysNo | int | 是 | 职位类型编码（分类） |
| PositionClasses| array[PositionClass] | 是 | 职位类型编码(从老祖先开始，一直到自己) |
| PositionName | Nvarchar\(50\) | 是 | 职位名称（冗余） |
| PositionType | int | 否 | 工作类型:0不限,1全职,2兼职 |
| SexType | int | 否 | 性别要求：0不限,1男，2女 |
| RecruitCount | int | 否 | 招聘人数 |
| ExperienceRequirements | int | 否 | 经验要求：0不限,1一年内，2一到三年，3三到五年，4五到十年，5十年以上 |
| Remark | Nvarchar\(max\) | 否 | 备注 |
| PositionPathList | array string | 否 | 工作地Path文件列表 |
| PositionUrlList | array string | 否 | 工作地Url文件列表 |
| PositionSalaryList | array object | 否 | 岗位薪资列表 |
| PositionAgeList | array object | 否 | 岗位年龄列表 |
| IfHasRecruit | int | 否 | 是否有招聘纪录0所有。1有，2无 |
| PositionWorkDayList | array object | 否 | 工作日期列表 |
| PositionWorkTimeList | array object | 否 | 工作时间列表 |


> #### PositionClass
| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionClassSysNo | int | 是 | 职位类型编码（分类）  |
| PositionClassName| string| 是 |职位类型名称  |



> #### 薪资 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionSalarySysNo | int | 是 | 系统编码 |
| SalaryType | int | 是 | 薪资类型：1月，2天，3时 |
| SalaryMax | Decimal\(18,2\) | 是 | 最大值 |
| SalaryMin | Decimal\(18,2\) | 是 | 最小值 |
| Remark | Nvarchar\(max\) | 否 | 备注 |

> #### 年龄 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionAgeSysNo | int | 是 | 系统编码 |
| AgeType | int | 是 | 年龄类型：0普通,1男,2女 |
| AgeMax | int | 是 | 最大值 |
| AgeMin | int | 是 | 最小值 |
| Remark | Nvarchar\(max\) | 否 | 备注 |

> #### 工作日期PositionWorkDay（兼职有效）

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionWorkDaySysNo | int | 是 | 工作日期系统编码|
| DayOfWeek | int | 是 | （0周日，1周一，2周二……6周六） |

> #### 工作时间点PositionWorkTime（兼职有效）

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionWorkTimeSysNo | int | 是 | 工作时间点系统编码|
| StartTime | datetime | 是 |开始时间 |
| EndTime | datetime | 是 |结算时间 |






> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### 功能按钮字段 {#请求数据}

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionSysNo | int | 否 | 职位系统编码 |
| OrganizationSysNo | int |否| 组织系统编码 |
| KeyWord | string | 否 | 关键字（名称） |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称） |
| IsMyFootPrint | int | 否 | 是否显示自己的：0否，1是（不传查全部，传值需通过UserSysNo匹配Person） |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowPositionUrlList | int | 否 | 是否显示工作地图片 |
| IsShowPositionSalaryList | int | 否 | 是否显示岗位薪资列表 |
| IsShowPositionAgeList | int | 否 | 是否显示岗位年龄列表 |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}




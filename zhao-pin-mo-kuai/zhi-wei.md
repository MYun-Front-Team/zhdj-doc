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
| PositionSalaryList | array object | 否 | 客户岗位薪资列表 |
| PositionAgeList | array object | 否 | 岗位年龄列表 |
| IfHasRecruit | int | 否 | 是否有招聘纪录0所有。1有，2无 |
| PositionWorkDayList | array object | 否 | 工作日期列表（星期） |
| PositionWorkTimeList | array object | 否 | 工作时间列表 |
| TagClassList | array object | 否 | 福利标签列表（说明见通用） |
| CustomerPositionName| Nvarchar\(50\) | 否 | 客户自定义职位名称 |
| PositionDayAreaList | array object | 否 | 工作日期列表（日期） |
|---------------- | ---------------- | ---------------- | ----------------|
| ShopName | string| 否 | 店铺 |
| SellerName| string| 否 | 商家名称|
| ContractAddress| string| 否 | 店铺地址 |
| PlatPositionSalaryList | array object | 否 | 平台可见岗位薪资列表 |
| InterviewBrand| string| 否 |面试品牌|
| InterviewPerson| string| 否 | 面试联系人 |
| InterviewPhone| string| 否 |面试联系人手机|
| InterviewPersonPost| string| 否 | 面试联系人职务 |
| InterviewAddress| string| 否 |面试联系人地址| 
| InterviewRemark| string| 否 | 面试备注 |
| ShopInterviewDateList | array ShopInterviewDate| 否 | 面试时间 |
| InterviewLongitude | decimal（18，10） | 否 | 面试经度 |
| InterviewLatitude | decimal（18，10） | 否 | 面试纬度 |
| Reward|decimal| 否 | 平台奖励|
|SalesManagerPersonSysNo| int | 否 |销售经理编码|
|SalesManagerPersonName| int | 否 |销售经理名称|
|IsHot| int | 否 |是否热门岗位|
|HotStartTime| datetime | 否 |热门开始|
|HotEndTime| int | 否 |热门结束|
|IsBonus| int | 否 |是否返佣|
|BonusAmount| decimal | 否 |返佣金额|


#### ShopInterviewDate

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StartDate| datetime| 是 |开始面试时间（只有时分秒有效）|
| EndDate| datetime| 是 |结束面试时间（只有时分秒有效） |


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

> #### 工作日期（星期）PositionWorkDay（兼职有效）

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
| TagClassSysNo | int | 是 | 福利编码（分类）  |
| TagClassName| string| 是 |福利名称  |








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
| IsShowPositionSalaryList | int | 否 | 是否显示客户岗位薪资列表 |
| IsShowPlatPositionSalaryList  | int | 否 | 是否显示平台岗位薪资列表 |
| IsShowPositionAgeList | int | 否 | 是否显示岗位年龄列表 |
| IsShowPositionWorkDayList | int | 否 | 是否显示工作日列表 |
| IsShowPositionWorkTimeList | int | 否 | 是否显示工作时间列表 |
| IsShowPositionDayAreaList  | int | 否 | 是否显示工作日期列表（日期）|
| IsShowTagClassList   | int | 否 | 是否显示福利列表 |






####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}




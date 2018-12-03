# 获取人员期望/现有职位和期望工资

##### _【功能说明】_ {#【功能说明】}

获取人员期望/现有职位和期望工资

_**【应用场景】**_

获取人员期望/现有职位和期望工资

_**【接口地址】**_

http://ip:port/RecruitQuery/Recruit/GetPersonRecruit
> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 |人员编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonPositions |array object | 是 | 基础字段 |
| PersonSalarys |array object | 否 | 统计字段 |
| ExpectPCDDescriptions|array string| 否 |期望工作省市区|
| ExpectAddresses | array[ExpectAddress] | 否 |期望工作地点 |
| FreeTimes| array[FreeTime] | 否 |空闲时间 |

#### ExpectAddress

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ExpectAddressSysNo | int | 是 | 系统编码 （0新增，非0编辑）|
| Longitude| decimal | 是 | 经度|
| Latitude| decimal | 是 |维度 |
| Address| string | 是 | 地址 |

#### FreeTime

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FreeTimeSysNo | int | 是 | 系统编码 （0新增，非0编辑）|
| TimeType| int | 否 | 标签类型：端自定义（任意时间、双休日……）|
| DayOfWeek| int | 否 |周几（1-7周1~周日） |
| StartTime| datetime| 是 | 开始时间（只有时分秒有效)|
| EndTime| datetime| 是 |结束时间（只有时分秒有效） |




#### PersonSalary

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSalaryRelationSysNo | int | 否 | 系统编码 |
| SalaryType| int | 是| 薪资类型：1月，2天，3时|
| SalaryMax| decimal| 是 |最大值|
| SalaryMin| decimal| 是 |最小值|
| Remark| string | 否 |备注|



#### PersonPosition

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonPositionRelationSysNo | int | 是 | 系统编码 |
| PositionClassSysNo | int | 是 | 职位编码 |
| PositionName | int | 是 | 职位名称 |
| PersonPositionType| int | 是 | 类型：1期望，10做过 |



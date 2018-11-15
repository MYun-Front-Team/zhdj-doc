# 获取简历

##### _【功能说明】_ {#【功能说明】}

获取简历

_**【应用场景】**_

获取简历  
查询Person表

_**【接口地址】**_

[http://ip:port/RecruitQuery/Resume/GetResumeList](http://ip:port/RecruitQuery/Resume/GetResumeList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| KeyWord | string | 否 | 姓名手机 |
| BeforePositionName | string | 否 | 曾经做过 |
| WorkingYear | int | 否 | 工作年数（以上） |
| IsInsuranceList | array\[int\] | 否 | 有无社保0无，1有 |
| LastCommunicateStatusList | array\[int\] | 否 | 最后沟通状态（端定义） |
| UserGenderList | array\[int\] | 否 | 性别：1男，2女 |
| Year | int | 否 | 年龄（以下） |
| EducationList | array\[int\] | 否 | 学历：0未知,1小学,2初中,3中转,4高中,5专科,6本科,7硕士,8博士,9其它 |
| ExpectPositionName | string | 否 | 期望岗位 |
| ExpectAddress | string | 否 | 期望工作地点 |
| IfInterviewList | array\[int\] | 否 | 是否有面试（0无 1有） |
| TimeTypeList | array\[int\] | 否 | 标签类型：端自定义（任意时间、双休日……） |
| DayOfWeekList | array\[int\] | 否 | 周几（1-7周1~周日） |
| StartTime | datetime | 否 | 开始时间（只有时分秒有效\) |
| EndTime | datetime | 否 | 结束时间（只有时分秒有效） |
| Longitude | decimal | 否 | 经度 |
| Latitude | decimal | 否 | 维度 |
| Distance | decimal | 否 | 距离 |
| SysJobStatusList |array[int] | 是 | 系统计算在职状态 （10在职 0不在职，1待面试）|


#### Resume

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Person | object | 是 | 人员（简版） |
| PersonPositionList | array object | 是 | 期望岗位列表（Limit） |
| PersonSalaryList | array object | 是 | 期望薪资列表（Limit） |
| ExpectPCDDescriptions | array\[string\] | 是 | 期望工作省市区 |
| ExpectAddresses | array\[ExpectAddress\] | 是 | 期望工作地点 |
| FreeTimes | array\[FreeTime\] | 是 | 空闲时间 |
| LastCommunicateStatus | int | 是 | 最后沟通状态（端定义） |
| LastCommunicateRemark | string | 是 | 最后沟通内容 |
| AdminStatus | int | 是 | 0待激活，1已激活 |
| Interviews | array\[Interview\] | 是 | 最近面试 |
| LastCommunicatePersonFromName | string | 是 | 最后沟通人 |
| SysJobStatus | int | 是 | 系统计算在职状态（10在职 0不在职，1待面试） |
| IsHealthyList|array[int] | 否 | 有无健康证|




#### Person

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员系统编码 |
| PersonName | string | 是 | 昵称 |
| RealName | string | 是 | 真实姓名 |
| UserGender | int | 是 | 性别：1男，2女 |
| BirthDay | string | 是 | 生日 |
| PCDCode | string | 是 | 省市区 |
| PCDDescription | string | 是 | 省市区 |
| ContractAddress | string | 是 | 地址 |
| CompanyName | string | 是 | 最近公司名称 |
| Post | string | 是 | 工作岗位 |
| IDCard | string | 是 | 身份证 |
| Nation | string | 是 | 民族 |
| Origin | string | 是 | 籍贯 |
| Education | int | 否 | 学历：0未知,1小学,2初中,3中转,4高中,5专科,6本科,7硕士,8博士,9其它 |
| FileUrlList | array string | 否 | 图片列表（首图为头像） |
| PersonProfile | string | 否 | 个人简介 |
| WorkingDate | string | 否 | 参加工作日期 |
| FileLifePathList | array string | 否 | 生活照图片列表 |
| BloodType | string | 否 | 血型 |
| Anaphylaxis | string | 否 | 过敏史 |
| Hobby | string | 否 | 爱好 |
| Remark | string | 否 | 备注 |
| IDCardType | int | 否 | 证件类型 |
| NeedPartTimeJob | int | 是 | 是否屏蔽推送兼职（0正常，1屏蔽） |
| CellPhoneNo | string | 是 | 手机号 |
| PersonProfile | string | 是 | 个人简介 |
| WorkingDate | string | 是 | 参加工作日期 |
| InSchoolStatus | int | 是 | 在校学生状态（0不明 1是 2不是） |
| NeedPartTimeJob | int | 是 | 是否屏蔽推送兼职（0正常，1屏蔽） |
| ExpectPCDDescriptions | array\[string\] | 是 | 期望工作省市区 |
| WorkingStatus | int | 是 | 工作状态：0离职，1在职，2观望 |
| ExpectPositionType | int | 是 | 期望工作类型:0不限,1全职,2兼职 |
| FreeTimeType | int | 是 | 空闲时间类型（1按标签2按星期） |
| CpsSysNo | int | 是 | CPS来源编码 |
| IsInsurance | int | 是 | 有无社保 |
| IsHealthy| int | 否 | 有无健康证|



#### PersonSalary

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSalaryRelationSysNo | int | 否 | 系统编码（0新增，非0编辑） |
| SalaryType | int | 是 | 薪资类型：1月，2天，3时 |
| SalaryMax | decimal | 是 | 最大值 |
| SalaryMin | decimal | 是 | 最小值 |
| Remark | string | 否 | 备注 |

#### PersonPosition

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonPositionRelationSysNo | int | 是 | 系统编码 （0新增，非0编辑） |
| PositionClassSysNo | int | 是 | 职位编码 |
| PersonPositionType | int | 是 | 类型：1期望，10做过 |
| PositionName | string | 是 | 职位名称 |

#### ExpectAddress

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ExpectAddressSysNo | int | 是 | 系统编码 （0新增，非0编辑） |
| Longitude | decimal | 是 | 经度 |
| Latitude | decimal | 是 | 维度 |
| Address | string | 是 | 地址 |

#### FreeTime

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FreeTimeSysNo | int | 是 | 系统编码 （0新增，非0编辑） |
| TimeType | int | 否 | 标签类型：端自定义（任意时间、双休日……） |
| DayOfWeek | int | 否 | 周几（1-7周1~周日） |
| StartTime | datetime | 是 | 开始时间（只有时分秒有效\) |
| EndTime | datetime | 是 | 结束时间（只有时分秒有效） |

### Interview

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InterviewSysNo | int | 是 | 面试系统编码 |
| InterviewName | string | 是 | 面试项目 |
| StartTime | datetime | 是 | 面试开始 |
| EndTime | string | 是 | 面试结束 |




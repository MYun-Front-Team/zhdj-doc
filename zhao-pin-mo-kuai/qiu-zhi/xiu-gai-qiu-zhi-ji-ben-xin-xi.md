# 修改求职基本信息 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改求职基本信息

_**【应用场景】**_

修改求职基本信息

注：基本信息保存到基础模块的Person里面，期望职位和薪资保存到招聘模块；

_**【接口地址】**_

[http://ip:port/RecruitAction/Recruit/](http://ip:port/HMAction/River/AddRiver)EditRecruitPerson

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 否 | 人员编码（如果不传则修改UserSysNo对应的Person） |
| PersonPositionList | array object | 否 | 期望职位列表 |
| PersonSalaryList | array object | 否 | 期望薪资列表 |
| WorkingStatus | int | 否 | 工作状态：0离职，1在职，2观望 |
| PersonName | string | 否 | 昵称 |
| RealName | string | 否 | 真实姓名 |
| UserGender | int | 否 | 性别：1男，2女 |
| BirthDay | string | 否 | 生日 |
| PCDCode | string | 否 | 省市区 |
| PCDDescription | string | 否 | 省市区 |
| ContractAddress | string | 否 | 地址 |
| CompanyName | string | 否 | 公司名称 |
| Post | string | 否 | 工作岗位 |
| IDCard | string | 否 | 身份证 |
| Nation | string | 否 | 民族 |
| Origin | string | 否 | 籍贯 |
| Education | int | 否 | 学历：0未知,1小学,2初中,3中转,4高中,5专科,6本科,7硕士,8博士,9其它 |
| FilePathList | array string | 否 | 头像图片列表 |
| FileLifePathList | array string | 否 | 生活照图片列表 |
| CellPhoneNo | string | 否 | 电话 |
| PersonProfile | string | 否 | 个人简介 |
| WorkingDate | string | 否 | 参加工作日期 |
| InSchoolStatus| int | 否 | 在校学生状态（0不明 1是 2不是） |
| NeedPartTimeJob| int | 否 | 是否屏蔽推送兼职（0正常，1屏蔽） |
| expectPCDDescriptions | array[string] | 否 |期望工作省市区 |
| ------------------ | ------------------ | ------------------ |------------------ |
| ExpectAddresses | array[ExpectAddress] | 否 |期望工作地点 |
| ExpectPositionType | int | 否 | 期望工作类型:0不限,1全职,2兼职 |
| FreeTimeType| int | int | 空闲时间类型（1按标签2按星期）|
| FreeTimes| array[FreeTime] | 否 |空闲时间 |
| CpsSysNo| int | 否 | CPS来源编码|
| IsInsurance| int | 否 | 有无社保|
| Height| decimal| 否 | 身高 |

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
| PersonPositionRelationSysNo | int | 是 | 系统编码 |
| PositionClassSysNo | int | 是 | 职位编码 |
| PersonPositionType | int | 是 | 类型：1期望，10做过 |
| PositionName | string | 是 | 职位名称 |

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


#### _应答数据_




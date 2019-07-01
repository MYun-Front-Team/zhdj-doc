# 获取面试列表
##### _【功能说明】_ {#【功能说明】}

获取面试列表


_**【应用场景】**_

获取面试列表


_**【接口地址】**_

http://ip:port/RecruitQuery/Interview/GetInterviewPersonList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InterviewPersonSysNo| int | 是 | 面试人员表编码 |
| InterviewSysNo| int | 否 | 面试编码|
| KeyWord| string| 否 | 姓名手机 |
| BeforePositionName | string | 否 | 曾经做过 |
| WorkingYear| int| 否 | 工作年数（以上） |
| IsInsuranceList|array[int] | 否 | 有无社保0无，1有|
| LastCommunicateStatusList| array[int] | 否 |最后沟通状态（端定义）|
| UserGenderList | array[int] | 否 | 性别：1男，2女 |
| Year| int| 否 | 年龄（以下） |
| ExpectPositionName | string | 否 | 期望岗位 |
| ExpectAddress| string  | 否 |期望工作地点 |
| Longitude| decimal | 否 | 经度|
| Latitude| decimal | 否 |维度 |
| Distance| decimal | 否 |距离|
| PersonStatusList | array[int] | 否 | 面试人员状态（0邀约，10通过，11未通过） |
| IsQuitList|array[int] | 否 | 是否离职|
| ShopSysNo| int | 否 | 店铺编码|
| PositionSysNo| int | 否 | 岗位编码|
| StartWorkStartDay|datetime| 否 | 开始预计入职时间|
| EndWorkStartDay|datetime| 否 | 结束预计入职时间|
| EntryStatusList|array[int] | 否 | 入职状态（0待入职10已入职11未入职）|
| StartEntryDate|datetime| 否 | 开始入职时间|
| EndEntryDate|datetime| 否 | 结束入职时间|
| OrganizationSysNo| int | 否 |组织编码 |
| PositionName | string  | 是 | 岗位名称 |
| InvitePersonName| int | 是 | 邀请人|
| StartCreateTime| datetime| 是 | 开始邀请时间|
| EndCreateTime| datetime| 是 | 结束邀请时间|
| StartInterviewStartTime| datetime| 否 | 起始面试时间|
| EndInterviewStartTime| datetime| 否 | 终止面试时间|
| NoPassTypeList|array[int] | 是 | 未通过原因，端定义 |
| PositionTypeList  |array[int] | 否 | 工作类型:0不限,1全职,2兼职 |
| StartQuitDate| datetime| 是 | 开始离职时间 |
| EndQuitDate| datetime| 是 | 结束离职时间 |
| DataRangeSysNo| int | 否 |店铺树编码 |
| SourceFrom| int | 否 |来源详情 |
| SettlementDate| datetime| 是 | 账期开始时间 |
| SettlementDateEnd| datetime| 是 | 账期结束时间 |
| InvitePersonAdminStatusList|array[int] | 否 | 邀请人状态（0待激活 1激活 2禁用） |
| InvitePersonDepartmentSysNo| int | 是 | 邀请人部门|
| FatherInvitePersonDepartmentSysNo| int | 是 | 邀请人部门和下属部门|
| InvitePersonSysNo| int | 是 | 邀请人编码|


#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InterviewPersonSysNo| int | 是 | 面试人员表编码 |
| PersonSysNo| int | 是 | 人员编码 |
| Person | object | 是 | 人员（简版） |
| ExpectPCDDescriptions | array[string] | 是 |期望工作省市区 |
| ExpectAddresses | array[ExpectAddress] | 是 |期望工作地点 |
| FreeTimes| array[FreeTime] | 是 |空闲时间 |
| LastCommunicateStatus| int | 是 |最后沟通状态（端定义）|
| LastCommunicateRemark| string | 是 |最后沟通内容 |
| LastCommunicatePersonFromName| string | 是 |最后沟通人 |
| InvitePersonName| int | 是 | 邀请人|
| CreateTime| datetime| 是 | 邀请时间|
| PersonStatus | int | 否 | 面试人员状态（0邀约，10通过，11未通过） |
| IsQuit|int| 否 | 是否离职|
| WorkStartDay|datetime| 否 | 预计入职时间|
| Salary|decimal| 否 | 薪水|
| Reward|decimal| 否 | 平台奖励|
| Position | Position| 是 | 岗位 |
| WorkStartRemark| string | 是 |描述 |
| NoPassType| int | 是 | 未通过原因，端定义 |
| NoPassRemark| string | 是 |未通过备注 |
| IsQuit| int | 是 | 是否离职 |
| QuitDate| datetime| 是 | 离职时间 |
| QuitType| int | 否 | 离职类型 |
| QuitReason| string| 是 | 离职原因  |
| QuitRemark| string| 否 | 离职备注 |
| EntryStatus|int | 否 | 入职状态（0待入职10已入职11未入职）|
| EntryDate|datetime| 否 | 入职时间 |
| EntryRemark|string| 否 | 入职备注 |
| ShopName | string| 否 | 店铺 |
| SellerName| string| 否 | 商家名称|
| SalaryUnit| int | 否 | 薪资单位枚举，端定义 |
| RewardUnit| int | 否 | 平台奖励单位枚举，端定义 |
| EntrySysDate|datetime| 否 | 录入日期 |
| InterviewStartTime| datetime| 是 |面试开始 |
| InterviewEndTime| datetime| 是 |面试结束|
| InterviewAddress| string| 是 |面试地址 |
| ----| ----|----|---- |
| WorkHour| int | 是 |工作小时数合计（SettlementDate传了有效） |
| OvertimeHour| int | 是 |固定加班小时数（SettlementDate传了有效） |
|GZOvertimeHour | int | 否 | 工作日加班时小时数（SettlementDate传了有效） |
| GXOvertimeHour| int | 否 | 公休日加班时小时数 （SettlementDate传了有效）|






#### Person

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int| 是 | 人员系统编码 |
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
| FileLifePathList| array string | 否 | 生活照图片列表 |
| BloodType| string| 否 | 血型|
| Anaphylaxis| string| 否 |过敏史|
| Hobby| string| 否 |爱好|
| Remark| string| 否 |备注|
| IDCardType | int| 否 | 证件类型|
| NeedPartTimeJob| int | 是 | 是否屏蔽推送兼职（0正常，1屏蔽） |
| CellPhoneNo| string | 是 |手机号 |
| PersonProfile | string | 是 | 个人简介 |
| WorkingDate | string | 是 | 参加工作日期 |
| InSchoolStatus| int | 是 | 在校学生状态（0不明 1是 2不是） |
| NeedPartTimeJob| int | 是 | 是否屏蔽推送兼职（0正常，1屏蔽） |
| ExpectPCDDescriptions | array[string] | 是 |期望工作省市区 |
| WorkingStatus | int | 是 | 工作状态：0离职，1在职，2观望 |
| ExpectPositionType | int | 是 | 期望工作类型:0不限,1全职,2兼职 |
| FreeTimeType| int | 是 | 空闲时间类型（1按标签2按星期）|
| CpsSysNo| int | 是 | CPS来源编码|
| IsInsurance| int |是 | 有无社保|




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


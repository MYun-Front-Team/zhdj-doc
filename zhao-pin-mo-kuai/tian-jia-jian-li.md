# 新增简历
##### _【功能说明】_ {#【功能说明】}

新增简历


_**【应用场景】**_

新增简历
1.查询[MY_BasicMgmt].[dbo].[T_Basic_Person]是否存在手机号一样的，存在报错，不存在，调用MyBizHelp.LoginHelp.Register
2.根据返回的PersonSysNo编辑人员信息
3.保存人员的期望工作，工资，期望地点


_**【接口地址】**_

http://ip:port/RecruitAction/Resume/AddResume

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonName | string | 是 | 昵称 |
| RealName | string | 是 | 真实姓名 |
| UserGender | int | 否 | 性别：1男，2女 |
| BirthDay | string | 否 | 生日 |
| PCDCode | string | 否 | 省市区 |
| PCDDescription | string | 否 | 省市区 |
| ContractAddress | string | 否 | 地址 |
| CompanyName | string | 否 | 最近公司名称 |
| Post | string | 否 | 工作岗位 |
| IDCard | string | 否 | 身份证 |
| Nation | string | 否 | 民族 |
| Origin | string | 否 | 籍贯 |
| Education | int | 否 | 学历：0未知,1小学,2初中,3中转,4高中,5专科,6本科,7硕士,8博士,9其它 |
| FileUrlList | array string | 否 | 图片列表（首图为头像） |
| PersonProfile | string | 否 | 个人简介 |
| WorkingDate | string | 否 | 参加工作日期 |
| Propertys | array object | 否 | 人员属性列表（见通用属性说明） |
| PrivacyPropertys | array object | 否 | 隐私属性列表 |
| TagSysNoList | array int | 否 | 标签列表 |
| IfVerify | int | 否 | 是否要连接三方查证身份证合法性 |
| FileLifePathList| array string | 否 | 生活照图片列表 |
| BloodType| string| 否 | 血型|
| Anaphylaxis| string| 否 |过敏史|
| Hobby| string| 否 |爱好|
| Remark| string| 否 |备注|
| IDCardType | int| 否 | 证件类型|
| NeedPartTimeJob| int | 否 | 是否屏蔽推送兼职（0正常，1屏蔽） |
| CellPhoneNo| string | 是 |手机号 |
| PersonProfile | string | 否 | 个人简介 |
| WorkingDate | string | 否 | 参加工作日期 |
| InSchoolStatus| int | 否 | 在校学生状态（0不明 1是 2不是） |
| NeedPartTimeJob| int | 否 | 是否屏蔽推送兼职（0正常，1屏蔽） |
| ExpectPCDDescriptions | array[string] | 否 |期望工作省市区 |
| WorkingStatus | int | 否 | 工作状态：0离职，1在职，2观望 |
| PersonPositionList | array object | 否 | 期望职位列表 |
| PersonSalaryList | array object | 否 | 期望薪资列表 |
| ExpectAddresses | array[ExpectAddress] | 否 |期望工作地点 |


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
| PersonPositionRelationSysNo | int | 是 | 系统编码 （0新增，非0编辑）|
| PositionClassSysNo | int | 是 | 职位编码 |
| PersonPositionType | int | 是 | 类型：1期望，10做过 |
| PositionName | string | 是 | 职位名称 |

#### ExpectAddress

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Longitude| decimal | 是 | 经度|
| Latitude| decimal | 是 |维度 |
| Address| string | 是 | 职位编码 |





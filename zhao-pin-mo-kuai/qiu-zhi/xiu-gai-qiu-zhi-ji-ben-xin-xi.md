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
| FileUrlList | array string | 否 | 图片列表（首图为头像） |
| PersonProfile | string | 否 | 个人简介 |
| WorkingDate | string | 否 | 参加工作日期 |

#### _应答数据_




# 修改党员 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改党员

_**【应用场景】**_

修改党员。

注：不传则不修改，修改记录要保留日志。

_**【接口地址】**_

[http://ip:port/PartyAction/Party/E](http://ip:port/HMAction/River/AddRiver)ditPartyMember

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PartyMemberSysNo | int | 是 | 党员系统编码 |
| MemberName | string | 否 | 姓名 |
| MemberGender | int | 否 | 性别：1男，2女 |
| IDCard | string | 否 | 身份证 |
| Nation | string | 否 | 民族 |
| Origin | string | 否 | 籍贯 |
| BirthDay | string | 否 | 出生年月 |
| Education | int | 否 | 教育 |
| PCDCode | string | 否 | 省市区 |
| PCDDescription | string | 否 | 省市区 |
| ContractAddress | string | 否 | 联系地址 |
| CompanyName | string | 否 | 公司名称 |
| WorkingDate | string | 否 | 参加工作时间 |
| Post | string | 否 | 岗位 |
| PersonFilePathList | array string | 否 | 人员文件path列表 |
| Remark | string | 否 | 备注 |
| DepartmentPost | int | 否 | 所属支部岗位 |
| PartyPost | int | 否 | 党内岗位 |
| OrganizationalStatus | int | 否 | 组织状态：0正常，1流动党员 |
| InnerPartyStatus | int | 否 | 党内状态：0入党积极分子，1预备党员，2正式党员 |
| IntroducerName | string | 否 | 介绍人编码 |
| PositiveMemberTime | string | 否 | 入党积极份子时间 |
| JoinPartyTime | string | 否 | 入党时间 |
| FullMemberTime | string | 否 | 转正时间 |
| RelationshipTransitTime | string | 否 | 关系转入时间 |
| AnchoredDepartmentSysNo | int | 否 | 挂靠支部编码 |
| DuesStandard | decimal | 否 | 党费标准 |
| DuesDate | string | 否 | 党费交至年月 |
| Remark | string | 否 | 备注 |
| IsOutOfContact | int | 否 | 是否失联党员 |
| OutOfContactDate | string | 否 | 失联时间 |
| OutwardFlow | string | 否 | 流动党员外出流向 |
| PartyFilePathList | array string | 否 | 党员文件path列表 |
| PersonIDPhotoPathList | array string | 否 | 证件照图片列表 |




# 导入党员 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

导入党员

_**【应用场景】**_

导入党员

注：先验证导入合法性，返回成功后，开始导入。

注：以免导入半途中断，每次导入如果系统有重复的数据，不能重复导入，尤其是person的唯一性判断。

_**【接口地址】**_

[http://ip:port/PartyAction/Party/Add](http://ip:port/HMAction/River/AddRiver)PartyMemberList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeName | int | 是 | 所属支部名称（中文） |
| MemberName | string | 是 | 姓名 |
| CellPhoneNo | string | 是 | 手机 |
| MemberGender | int | 否 | 性别：1男，2女 |
| IDCard | string | 否 | 身份证 |
| Nation | string | 否 | 民族 |
| Origin | string | 否 | 籍贯 |
| BirthDay | string | 否 | 出生年月 |
| EducationStr | string | 否 | 教育（中文） |
| ContractAddress | string | 否 | 联系地址 |
| CompanyName | string | 否 | 公司名称 |
| WorkingDate | string | 否 | 参加工作时间 |
| Post | string | 否 | 工作岗位 |
| InnerPartyStatusStr | int | 是 | 党内状态（中文）：0入党积极分子，1预备党员，2正式党员 |
| PositiveMemberTime | string | 否 | 入党积极份子时间 |
| JoinPartyTime | string | 否 | 入党时间 |
| FullMemberTime | string | 否 | 转正时间 |
| DuesStandard | decimal | 否 | 党费标准 |
| DuesDate | string | 否 | 党费交至年月 |
| IsOutOfContactStr | string | 是 | 是否失联党员（中文）：否，是 |
| OutOfContactDate | string | 否 | 失联时间 |
| OrganizationalStatusStr | string | 是 | 是否流动党员（中文）：否，是 |
| OutwardFlow | string | 否 | 流动党员外出流向 |

#### _应答数据_ {#应答数据-}




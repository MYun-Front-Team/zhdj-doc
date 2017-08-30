# 获取党员详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取党员详情

_**【应用场景】**_

获取党员详情

_**【接口地址】**_

[http://ip:port/DMQuery/Party/GetPartyMember](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)BySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberSysNo | int | 是 | 党员系统编码 |
| IsShowUser | int | 否 | 是否显示用户 |
| IsShowLogList | int | 否 | 是否显示日志 |
| LogTypeList | array int | 否 | 日志类型：党费、流转等 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberSysNo | int | 是 | 党员编码 |
| DepartmentSysNo | int | 否 | 所属支部编码 |
| MemberName | string | 否 | 姓名 |
| CellPhoneNo | string | 否 | 手机 |
| MemberGender | int | 否 | 性别：1男，2女 |
| IDCard | string | 否 | 身份证 |
| Nation | string | 否 | 民族 |
| Origin | string | 否 | 籍贯 |
| BirthDay | string | 否 | 出生年月 |
| Education | int | 否 | 教育 |
| ContractAddress | string | 否 | 联系地址 |
| Post | string | 否 | 岗位 |
| Remark | string | 否 | 备注 |
| PartyPost | string | 否 | 党内岗位 |
| OrganizationalStatus | int | 否 | 组织状态：0正常，1流动党员 |
| InnerPartyStatus | int | 否 | 党内状态：0入党积极分子，1预备党员，2正式党员 |
| IntroducerSysNo | int |  | 介绍人编码 |
| PositiveMemberTime | string | 否 | 入党积极份子时间 |
| JoinPartyTime | string | 否 | 入党时间 |
| FullMemberTime | string | 否 | 转正时间 |
| RelationshipTransitTime | string | 否 | 关系转入时间 |
| AnchoredDepartmentSysNo | int | 否 | 挂靠支部编码 |
| DuesStandard | decimal | 否 | 党费标准 |
| DuesDate | string | 否 | 党费交至年月 |
| User | object | 否 | 用户实体（见后台接口） |
| LogList | array object | 否 | 日志列表 |

#### LogList说明_ _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LogSysNo | int | 是 | 编码 |
| SourceType | int | 是 | 日志类型 |
| ActionTime | string | 是 | 操作时间 |
| ActionType | int | 是 | 操作动作类型 |
| ActionName | string | 是 | 操作名称 |
| ActionDescription | string | 否 | 操作描述 |




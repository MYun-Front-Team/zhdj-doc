# 党员模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MemberSysNo | int | 是 | 党员编码 |
| PersonSysNo | int | 是 | 人员编码 |
| DataRangeSysNo | int | 是 | 数据范围树编码\(所属支部\) |
| BranchDataRangeSysNo | int | 否 | 数据范围树编码\(所属党委，关联党内岗位\) |
| PartyPost | int | 否 | 党内职务：0党员,1书记，2副书记，3组织委员，4宣传委员 |
| OrganizationalStatus | int | 是 | 组织状态：0正常，1流动党员 |
| InnerPartyStatus | int | 是 | 党内状态：0入党积极分子，1预备党员，2正式党员 |
| IntroducerName | string | 是 | 介绍人姓名 |
| PositiveMemberTime | string | 是 | 入党积极份子时间 |
| JoinPartyTime | string | 是 | 入党时间 |
| FullMemberTime | string | 是 | 转正时间 |
| RelationshipTransitTime | string | 否 | 关系转入时间 |
| AnchoredDepartmentSysNo | int | 否 | 挂靠支部编码 |
| DuesStandard | decimal | 是 | 党费标准 |
| DuesDate | string | 是 | 党费交至年月 |
| Remark | string | 否 | 备注 |
| PartyPerson | object | 是 | 党员的人员实体对象 |
| FilePathList | array string | 否 | 文件图片Path路径（第一张为头像） |
| FileUrlList | array string | 否 | 文件图片Url路径（第一张为头像） |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LastActivityTime | string | 否 | 最近参数活动时间 |
| LastStudyTime | string | 否 | 最近学习时间 |
| LastReportTime | string | 否 | 最近汇报时间 |
| PointsValue | int | 否 | 积分值 |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AddPartyMember | 操作 | 是 | 新增党员 |
| EditPartyMember | 操作 | 是 | 修改党员 |
| AddPartyMemberMoveIn | 操作 | 是 | 转入（支部间） |
| AddPartyMemberMoveOut | 操作 | 是 | 转出（支部间） |
| GetPartyMemberList | 搜索 | 是 | 搜索党员列表 |
| GetPartyMemberBySysNo | 查询 | 是 | 根据编码，获取党员详情 |
| GetPartyMemberHonorList | 查询 | 是 | 查询党员荣誉列表 |

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 数据范围树枝叶编码 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（姓名、手机号） |
| PartyMemberSysNo | int | 否 | 党员系统编码 |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowImgUrlList | int | 否 | 是否显示图片列表 |
| IsShowFileUrlList | int | 否 | 是否显示文件列表 |
| IsShowPointsValue | int | 否 | 是否显示积分 |
| IsShowModuleRelationList | int | 否 | 是否显示模块关联列表 |
|  |  |  |  |

####  {#应答数据-（巡河记录数组）}

####  {#应答数据-（巡河记录数组）}




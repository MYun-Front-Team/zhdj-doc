# 招聘模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitSysNo | int | 是 | 招聘系统编码 |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 否 | 所属数据范围树 |
| ShopSysNo | int | 否 | 店铺系统编码 |
| ShopName| string | 否 | 店铺名称 |
| ContractAddress| string | 否 | 店铺地址 |
| Distance| decimal| 否 | 距离（IsMyFootPrint=1才有效） |
| AuditStatus | int | 是 | 审核状态：0待审核，10审核通过，11审核失败 |
| Position | object | 是 | 职位 |
| StartDate | string | 是 | 开始时间 |
| EndDate | string | 是 | 结束时间 |
| RecruitStatus | int | 是 | 招聘状态：0新建,10发布，11撤下 |
| EndSecond| double| 是 | 距离结束时间（秒）|
 

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitPersonTotalCount | int | 否 | 圈中人数 |
| RecruitPersonRobCount | int | 否 | 意向人数（已抢） |
| RecruitInstantStatus | int | 否 | 招聘即时状态：1未开始，2进行中，3已结束 |
| RecruitPerson | object | 否 | 应聘人员状态信息（IsShowMyPersonStatus=1） |

#### RecruitPerson
| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitSysNo| int | 否 | 招聘系统编码 |
| RecruitPersonStatus| int | 否 | 状态：0圈中，1已抢，2忽略，10抢中，11已失效 |
| RecruitPersonTime| Datetime| 否 | 抢的时间 |
| PositionSalary| decimal| 否 |岗位最终薪资 |
| SalaryType| Int| 否 |薪资类型：1月，2天，3时 |
| WorkStartDay| Datetime| 否 |开始上班时间 |





> #### 功能按钮字段 {#请求数据}

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitSysNo | int | 否 | 招聘系统编码 |
| OrganizationSysNo | int | 否 | 组织系统编码 |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称） |
| IsMyFootPrint | int | 否 | 是否显示自己的：0否，1是（不传查全部，传值需通过UserSysNo匹配Person） |
| PersonPositionTypeList | array int | 否 | 人员期望职位类型：1期望，10做过（Limit开关） |
| PositionSysNo| aint | 否 | 岗位编码 |



> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowRecruitPersonTotalCount | int | 否 | 是否显示圈中人数 |
| IsShowRecruitPersonRobCount | int | 否 | 是否显示意向人数 |
| IsShowRecruitInstantStatus | int | 否 | 是否显示招聘即时状态 |
| IsShowMyPersonStatus | int | 否 | 是否显示当前人员的参与情况 |
| IsShowPersonPositionList | int | 否 | 是否显示期望职位列表 |
| IsShowPersonSalaryList | int | 否 | 是否显示期望薪资列表 |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}




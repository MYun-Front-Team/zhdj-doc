# 招聘模块-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitSysNo | int | 是 | 招聘系统编码 |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 否 | 所属数据范围树 |
| ShopSysNo | int | 否 | 店铺系统编码 |
| ShopName| string | 否 | 店铺名称 |
| SellerName| string | 否 | 商家名称 |
| ContractAddress| string | 否 | 店铺地址 |
| Distance| decimal| 否 | 距离（IsMyFootPrint=1或查询条件传了经纬度有效） |
| AuditStatus | int | 是 | 商家审核状态：0待审核，10审核通过，11审核失败 |
| Position | object | 是 | 职位 |
| StartDate | string | 是 | 开始时间 |
| EndDate | string | 是 | 结束时间 |
| RecruitStatus | int | 是 | 招聘状态：0新建,10发布，11撤下 |
| EndSecond| double| 是 | 距离结束时间（秒）|
| SellerBossPersonSysNo| int | 否 | 店铺老板编码 |
| CustomerShopName| string| 是 | 客户名称 |
| CustomerSalary| decimal| 否 |客户薪资 |
| Commission| decimal| 否 |佣金 |
| Subsidy| decimal| 否 |补贴|
| CommissionType| int| 否 |佣金类型（不限制，端自定义） |
| PushLeaderEndTime| datetime| 否 |领队推送结束时间|
| PushLeaderStatus| int| 否 |推送领队状态（0待推送 10已推送） |
| InUser| string| 是 | 发布人|
| LeaderOnStatus| int| 否 |领队上下架状态（0待上架 1上架，2下架） |
| CommissionType| int| 否 |佣金类型（不限制，端自定义） |
| IsAgent| int| 否 |是否代理 |
| AgentRecruitShops| array RecruitShop | 否 |代理招聘的店铺组织 |
| SettlementType| int| 否 | 结算方式：1月结、2周结、3日结，4次日结，5完工结 |
| SettlementCycle| int| 否 | 结算周期 |
| IsShowInCommission| int| 否 | 是否在佣金推送列表显示 |
| OpenStatus | int | 是 | 开店状态：0待装修，10开，11关 |
| CommissionRemark| string| 否 |佣金备注 |
| RecruitAuditStatus| int| 否 |岗位审核状态（0待审核 10已经审核 11审核不通过） |
| AuditRemark| string| 否 |HR审核备注 |
| PlatAuditStatus| int | 否 |岗位平台审核状态（0待审核 10已经审核 11审核不通过） |
| PlatAuditRemark| int | 否 |岗位平台审核备注 |
| PlatAuditPersonName| string| 否 |岗位平台审核人 |
| RecruitNeedPlatAudit| int | 否 |发布岗位是否需要平台审核|
| PlatPositionSalaryStatus | int | 否 | 平台可见岗位薪资状态（0待设置，10已设置） |

> #### RecruitShop

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 招聘商家组织系统编码 |
| DataRangeSysNo | int | 否 | 招聘商家所属数据范围树 |
| ShopName| string| 否 | 招聘商家店铺名称|
| SaleName| string| 否 | 招聘商家商铺名称|


 

 

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitPersonTotalCount | int | 否 | 圈中人数 |
| RecruitPersonRobCount | int | 否 | 意向人数（报名总人数） |
| RecruitInstantStatus | int | 否 | 招聘即时状态：0岗位待审核 1未开始，2进行中，3已结束，4已过期 |
| RecruitPerson | object | 否 | 应聘人员状态信息（IsShowMyPersonStatus=1） |
| LeaderSuccessCount| int | 否 | 领队成功录用人数 |
| SuccessCount| int | 否 | 成功录用人数(发OFFER人数) |
| GoToWrokCount| int | 否 | 已入职人数 |
| RefuseCount| int | 否 |拒绝人数 |
| NoComeCount| int | 否 |放鸽子人数 |
| PickCount| int | 否 |已抢人数（待面试） |
| TakeInCount| int | 否 |线上已录用人数 |
| InvalidCount| int | 否 |失效人数 |
| FavoriteCount| int| 是 | 收藏数 |
| CancelCount| int | 否 |已取消人数（不确认OFFER人数和取消面试人数和） |
| WaitGoToWrokCount| int | 否 | 待入职人数 |
| InterviewPersonCount| int | 否 | 后台面试人数 |
| IsFavorite| int| 否 | 是否收藏夹的 |
| InterviewTakeInCount| int| 否 |线下已录用|
| InterviewGoToWrokCount| int| 否 |线下已入职人数|
| InterviewPickCount| int | 否 |线下已抢人数（待面试） |


#### RecruitPerson
| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitSysNo| int | 否 | 招聘系统编码 |
| RecruitPersonStatus| int | 否 | 状态：0圈中，1已抢，2忽略，10抢中，11已失效，12拒绝，19待入职（C接受Offer），20已上班，21放鸽子，22取消（C不接受Offerr和C取消面试）,30离职 |
| RecruitPersonTime| Datetime| 否 | 抢的时间 |
| PositionSalary| decimal| 否 |岗位最终薪资 |
| SalaryType| Int| 否 |薪资类型：1月，2天，3时 |
| WorkStartDay| Datetime| 否 |开始上班时间 |
| UrgeCount| int| 否 |催促次数 |
| Remark| string| 否 |备注|
| LeaderPersonSysNo| int| 否 | 邀请人 |
| InviterType| int| 否 | 邀请类型（0好友邀请，1分享邀请） |
| NoComeRemark| string| 是 | 放鸽子备注 |
| NoComeType| int| 是 | 自定义枚举备注 |
| CancelStatus| int| 是 | 取消状态（0正常，10取消） |
| CancelRemark| string| 是 | 取消备注 |
| HandleOfferStatus|int | 否 | Offer处理状态（0初始 1待处理 10通过，11不通过）|
| HandleOfferRmark|string | 否 | Offer处理备注|
| CancelCount| int| 否 |该岗位已经取消过的次数 |
| InterviewBrand| string| 否 |面试品牌|
| InterviewPerson| string| 否 | 面试联系人 |
| InterviewPhone| string| 否 |面试联系人手机|
| InterviewPersonPost| string| 否 | 面试联系人职务 |
| InterviewAddress| string| 否 |面试联系人地址| 
| InterviewRemark| string| 否 | 面试备注 |
| ShopInterviewDateList | array ShopInterviewDate| 否 | 面试时间 |
| InterviewLongitude | decimal（18，10） | 否 | 面试经度 |
| InterviewLatitude | decimal（18，10） | 否 | 面试纬度 |
| IsQuit| int| 是 | 是否离职（0正常，1离职） |
| QuitDate| datetime| 是 | 离职时间 |



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
| RecruitPersonStatus| int | 否 | 状态：0圈中，1已抢，2忽略，10抢中，11已失效，12拒绝，19待入职（C接受Offer），20已上班，21放鸽子，22取消（C不接受Offerr和C取消面试）  |
| RecruitPersonStatusList|array[int] | 否 | 状态：0圈中，1已抢，2忽略，10抢中，11已失效，12拒绝，19待入职（C接受Offer），20已上班，21放鸽子，22取消（C不接受Offerr和C取消面试）  |
| LeaderPickStatus| int| 否 |领队接单状态（0未接 1已接）和IsMyFootPrint，RecruitPersonStatus 不能共存 |
| IsLeaderPrint | int | 否 | 是否显示领队自己拉来的人：（0否，1是）和IsMyFootPrint不能共存 |
| PositionTypeList |array[int] | 否 | 工作类型:0不限,1全职,2兼职 |
| LeaderOnStatusList| array[int]| 否 |领队上下架状态（0待上架 1上架，2下架） | 
| PushLeaderStatusList| array[int]| 否 |推送领队状态（0待推送 10已推送） |
| RecruitInstantStatusList | int | 否 | 招聘即时状态：0岗位待审核 1未开始，2进行中，3已结束，4已过期 |
| IsAgentList|array int| 否 |是否代理 |
| RecruitStatusList | array int | 否 | 招聘状态：0新建,10发布，11撤下  |
| IsShowInCommissionList|array int| 否 | 是否在佣金推送列表显示 |
| LeaderPersonSysNo| int| 否 | 邀请人 |
|IfHasLeaderPersonOnly| int| 否 | 是否只显示有邀请人的 |
| IsShowRefuse| int| 否 | 是否显示商家主动拒绝的人 |
| ShopCloseHidden| int| 否 | 隐藏关店的招聘|
| RecruitAuditStatusList|array int| 否 |岗位审核状态（0待审核 10已经审核 11审核不通过） |
| PlatAuditStatusList| array int | 否 |岗位平台审核状态（0待审核 10已经审核 11审核不通过） |
| HandleOfferStatusList|Array[int] | 否 | Offer处理状态（0初始 1待处理 10通过，11不通过）|
| IsFavorite| int| 否 | 是否显示收藏夹的 |
| InterviewStaus| int| 否 | 面试状态（1即将面试 2待处理 3已完成） |
| IsMyOffer| int| 否 | 是否查看我的Offer(包括待入职和抢中，排除已取消) |
| IsOverdueList| int| 是 | 是否过期（0未过期 1已过期） |
| ShowFavoritePerson| int| 否 | 是否只显示收藏的人 |
| NotEqualRecruitSysNo| int | 否 | 排除招聘系统编码 |
| StartRecruitPersonTime| datetime| 否 |客户抢的时间开始 |
| EndRecruitPersonTime| datetime| 否 | 客户抢的时间结束 |
| StartApplyInterviewTime|datetime| 否 |面试申请时间开始 |
| EndApplyInterviewTime|datetime| 否 | 面试申请时间结束 |
| CancelStatusList|array int| 是 | 面试申请取消状态（0正常，10取消） |
| StartWorkStartDay|datetime| 否 |预计入职时间开始 |
| EndWorkStartDay|datetime| 否 | 预计入职时间结束 |
| Remark|string| 否 | 面试备注 |
| CancelOrHandleOfferRemark|string| 否 | 客户取消或拒绝Offer备注 |
| Latitude|decimal| 否 | 纬度（后台需求总览需要） |
| Longitude|decimal| 否 | 经度（后台需求总览需要） |
| CustomerPositionName| Nvarchar\(50\) | 否 | 客户自定义职位名称 |
| IsQuitList|array int| 是 | 是否离职（0正常，1离职） |
| PlatPositionSalaryStatusList |array[int] | 否 | 平台可见岗位薪资状态（0待设置，10已设置） |
| LeaderAdminStatusList|array[int] | 否 | 邀请人状态（0待激活 1激活 2禁用） |
| SalesManagerPersonSysNo| int | 否 |销售经理系统编码| 
| SalesManagerDepartmentSysNo| int| 否 |交付当前部门|
| FatherSalesManagerDepartmentSysNo| int | 否 |交付当前部门或下属部门| 
| IsShowPublic| int | 是 |限制交付人后，是否同时展示公海和潜客 |



> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowRecruitPersonTotalCount | int | 否 | 是否显示圈中人数 |
| IsShowRecruitPersonRobCount | int | 否 | 是否显示意向人数 |
| IsShowRecruitInstantStatus | int | 否 | 是否显示招聘即时状态 |
| IsShowMyPersonStatus | int | 否 | 是否显示当前人员的参与情况 |
| IsShowPersonPositionList | int | 否 | 是否显示期望职位列表 |
| IsShowPersonSalaryList | int | 否 | 是否显示期望薪资列表 |
| IsShowLeaderSuccessCount | int | 否 | 是否显示领对成功招募人数 |
| IsShowAgentRecruitShopsList | int | 否 | 是否显示代理招聘的店铺组织 |








####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}




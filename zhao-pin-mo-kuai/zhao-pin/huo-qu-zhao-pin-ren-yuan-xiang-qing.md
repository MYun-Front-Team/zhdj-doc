# 获取招聘人员列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取招聘人员列表

_**【应用场景】**_

获取招聘人员列表

_**【接口地址】**_

[http://ip:port/RecruitQuery/Recruit/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Recruit](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)PersonBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitPersonSysNo | int| 否 | 招聘详情记录编码 |
| Limit | object | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitPersonSysNo | int| 否 | 招聘详情记录编码 |
| RecruitPerson | object | 是 | 招聘人员 |
| RecruitPersonStatus| int | 否 | 状态：0圈中，1已抢，2忽略，10抢中，11已失效，12拒绝，19待入职（C接受Offer），20已上班，21放鸽子，22取消（C不接受Offerr和C取消面试）,30离职 |
| RecruitPersonTime | string | 否 | 抢的时间 |
| PositionSalary | decimal\(18,2\) | 否 | 岗位最终薪资 |
| SalaryType | int | 否 | 薪资类型：1月，2天，3时 |
| WorkStartDay | string | 否 | 开始上班时间 |
| Remark | string | 否 | 备注 |
| LeaderPersonSysNo| int| 否 | 邀请人 |
| LeaderAdminStatus| int| 否 | 邀请人账号状态（0待激活1激活2禁用） |
| LeaderCellPhoneNo| string| 否 | 邀请人电话 |
| LeaderRealName| string| 否 | 邀请人姓名 |
| InviterType| int| 否 | 邀请类型（0好友邀请，1分享邀请） |
| NoComeRemark| string| 是 | 放鸽子备注 |
| NoComeType| int| 是 | 自定义枚举备注 |
| RefusePersonSysNo| int| 是 | 拒绝人编码|
| RefusePersonName| string| 是 | 拒绝人名称|
| RefuseTime| string| 是 | 拒绝时间|
| SuccessPersonSysNo| int| 是 | 发OFFER人编码|
| SuccessPersonName| string| 是 | 发OFFER名称|
| SuccessTime| string| 是 | 发OFFER时间|
| GoToWrokPersonSysNo| int| 是 | 确认上班人编码|
| GoToWrokPersonName| string| 是 | 确认上班人名称|
| GoToWrokTime| string| 是 |确认上班人时间|
| ApplyInterviewTime| datetime| 否 | 面试申请时间 |
| CancelStatus| int| 是 | 取消状态（0正常，10取消） |
| CancelRemark| string| 是 | 取消备注 |
| HandleOfferStatus|int | 否 | Offer处理状态（0初始 1待处理 10通过，11不通过）|
| HandleOfferTime|datetime| 否 | Offer处理时间|
| HandleOfferRmark|string | 否 | Offer处理备注|
| IsOverdue| int| 是 | 是否过期（0未过期 1已过期） |
| IsDove| int | 是 | 是否放鸽子 |
| IsFavorite| int| 否 | 是否收藏夹的 |
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
| RecruitCertificateName| string| 否 | 签约服务商名称 |







#### RecruitPerson说明_ _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Person | object | 是 | 人员（简版） |
| DoveCount| int | 是 | 鸽子数 |
| Distance| decimal\(18,2\) | 否 | 距离店铺距离 |
| PersonPositionList | array object | 否 | 期望岗位列表（Limit） |
| PersonSalaryList | array object | 否 | 期望薪资列表（Limit） |




# 获取招聘人员列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取招聘人员列表

_**【应用场景】**_

获取招聘人员列表

_**【接口地址】**_

[http://ip:port/RecruitQuery/Recruit/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Recruit](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)PersonList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Query | object | 是 | 查询条件 |
| Limit | object | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitPersonSysNo | int| 否 | 招聘详情记录编码 |
| RecruitPerson | object | 是 | 招聘人员 |
| RecruitPersonStatus| int | 否 | 状态：0圈中，1已抢，2忽略，10抢中，11已失效，12拒绝，20已上班，21放鸽子 |
| RecruitPersonTime | string | 否 | 抢的时间 |
| PositionSalary | decimal\(18,2\) | 否 | 岗位最终薪资 |
| SalaryType | int | 否 | 薪资类型：1月，2天，3时 |
| WorkStartDay | string | 否 | 开始上班时间 |
| Remark | string | 否 | 备注 |
| LeaderPersonSysNo| int| 否 | 邀请人 |
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
| ShopName| string | 否 | 店铺名称 |
| SellerName| string | 否 | 商家名称 |
| CustomerPositionName| Nvarchar\(50\) | 否 | 客户自定义职位名称 |
| PositionName | Nvarchar\(50\) | 是 | 职位名称（冗余） |















#### RecruitPerson说明_ _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Person | object | 是 | 人员（简版） |
| Distance| decimal\(18,2\) | 否 | 距离店铺距离 |
| PersonPositionList | array object | 否 | 期望岗位列表（Limit） |
| PersonSalaryList | array object | 否 | 期望薪资列表（Limit） |




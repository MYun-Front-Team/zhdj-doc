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
| RecruitPersonStatus| int | 否 | 状态：0圈中，1已抢，2忽略，10抢中，11已失效，12拒绝，20已上班 |
| RecruitPersonTime | string | 否 | 抢的时间 |
| PositionSalary | decimal\(18,2\) | 否 | 岗位最终薪资 |
| SalaryType | int | 否 | 薪资类型：1月，2天，3时 |
| WorkStartDay | string | 否 | 开始上班时间 |
| Remark | string | 否 | 备注 |
| LeaderPersonSysNo| int| 否 | 邀请人 |





#### RecruitPerson说明_ _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Person | object | 是 | 人员（简版） |
| Distance| decimal\(18,2\) | 否 | 距离店铺距离 |
| PersonPositionList | array object | 否 | 期望岗位列表（Limit） |
| PersonSalaryList | array object | 否 | 期望薪资列表（Limit） |



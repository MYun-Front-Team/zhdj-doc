# 获取个人学历列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取个人学历列表

_**【应用场景】**_

获取个人学历列表

_**【接口地址】**_

[http://ip:port/BasicQuery/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/G](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etPersonEducationList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员编码（如果不传则获取UserSysNo对应的Person） |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| EducationSysNo | int | 是 | 系统编码 |
| EducationSchool | string | 是 | 学校 |
| EducationMajor | string | 是 | 专业 |
| EducationStartDate | string | 是 | 开始时间 |
| EducationEndDate | string | 是 | 结束时间 |
| EducationDesc | string | 否 | 描述 |
| Remark | string | 否 | 备注 |




# 修改个人学历 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改个人学历

_**【应用场景】**_

修改个人学历

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditPersonEducation

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| EducationSysNo | int | 是 | 学历系统编码 |
| EducationSchool | string | 是 | 学校 |
| EducationMajor | string | 是 | 专业 |
| EducationStartDate | string | 是 | 开始时间 |
| EducationEndDate | string | 是 | 结束时间 |
| EducationDesc | string | 否 | 描述 |
| Remark | string | 否 | 备注 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




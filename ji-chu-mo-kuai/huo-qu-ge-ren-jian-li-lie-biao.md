# 获取个人简历列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取个人简历列表

_**【应用场景】**_

获取个人简历列表

_**【接口地址】**_

[http://ip:port/BasicQuery/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/G](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etPersonResumeList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员系统编码 |
| IsOwner | int | 否 | 是否查询自己（该值存在的时候，人员编码可为空） |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ResumeSysNo | int | 是 | 系统编码 |
| ResumeStartDate | string | 是 | 简历开始时间 |
| ResumeEndDate | string | 是 | 简历结束时间 |
| ResumeDesc | string | 是 | 描述 |
| Remark | string | 否 | 备注 |




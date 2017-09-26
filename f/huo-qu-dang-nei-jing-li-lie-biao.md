# 获取党内经历列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取党内经历列表

_**【应用场景】**_

获取党内经历列表

_**【接口地址】**_

[http://ip:port/PartyQuery/Party/GetP](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)artyExperienceList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PartyMemberSysNo | int | 是 | 党员系统编码 |

#### _应答数据 \(数组\)_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ExperienceSysNo | int | 是 | 系统编码 |
| ExperienceDate | string | 是 | 时间 |
| ExperienceDesc | string | 是 | 内容 |




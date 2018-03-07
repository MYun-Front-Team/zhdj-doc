# 设置志愿者状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置志愿者状态

_**【应用场景】**_

设置志愿者状态

注：写入通用审核记录；

_**【接口地址】**_

[http://ip:port/ResidentAction/Volunteer/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etVolunteerStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| VolunteerSysNo | int | 是 | 系统编码 |
| VolunteerStatus | int | 是 | 志愿者状态：10审核通过，11审核失败 |
| Remark | string | 否 | 理由（拒绝时必填） |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




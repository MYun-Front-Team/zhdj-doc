# 确认抢班

##### _【功能说明】_ {#【功能说明】}

确认抢班

_**【应用场景】**_

确认抢班

注：人员如果为空，那么就用操作人的PersonSysNo；

_**【接口地址】**_

[http://ip:port/RecruitAction/Recruit/](http://ip:port/HMAction/River/AddRiver)SetRecruitPersonSuccess

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitSysNo | int | 是 | 招聘系统编码 |
| PersonSysNo | int | 否 | 人员系统编码 |
| LeaderPersonSysNo| int| 否 | 邀请人 |
| ApplyInterviewTime| datetime| 否 | 面试申请时间 |





#### _应答数据_ {#应答数据-}




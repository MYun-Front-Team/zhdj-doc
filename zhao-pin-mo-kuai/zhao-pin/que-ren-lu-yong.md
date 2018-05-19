# 确认录用 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

确认录用

_**【应用场景】**_

确认录用

注：同一个人如果存在其它的已抢招聘信息（进行中），那么标记RecruitPersonStatus=11；

_**【接口地址】**_

[http://ip:port/RecruitAction/Recruit/](http://ip:port/HMAction/River/AddRiver)SetRecruitSuccess

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitSysNo | int | 是 | 招聘系统编码 |
| PersonSysNo | int | 是 | 人员系统编码 |
| PositionSalary | decimal\(18,2\) | 是 | 岗位最终薪资 |
| SalaryType | int | 是 | 薪资类型：1月，2天，3时 |
| WorkStartDay | string | 是 | 开始上班时间 |

#### _应答数据_ {#应答数据-}




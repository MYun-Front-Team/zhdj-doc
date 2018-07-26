#批量录用

##### _【功能说明】_ {#【功能说明】}

批量录用

_**【应用场景】**_

批量录用


_**【接口地址】**_

[http://ip:port/RecruitAction/Recruit/](http://ip:port/HMAction/River/AddRiver)GroupSetRecruitSuccess

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitSysNo | int | 是 | 招聘系统编码 |
| PositionSalary | decimal\(18,2\) | 是 | 岗位最终薪资 |
| SalaryType | int | 是 | 薪资类型：1月，2天，3时 |
| WorkStartDay | string | 是 | 开始上班时间 |
| Remark | string | 是 | 备注 |
| PersonSysNoList |array int | 是 | 人员系统编码 |


#### _应答数据_ {#应答数据-}




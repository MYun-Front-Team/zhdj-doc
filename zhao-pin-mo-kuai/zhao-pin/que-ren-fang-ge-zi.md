# 确认放鸽子

##### _【功能说明】_ {#【功能说明】}

确认放鸽子

_**【应用场景】**_

确认放鸽子

注：只有已经确认录用的，才能确认放鸽子

_**【接口地址】**_

[http://ip:port/RecruitAction/Recruit/SetNoCome](http://ip:port/RecruitAction/Recruit/SetNoCome)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitSysNo | int | 是 | 招聘系统编码 |
| PersonSysNoList | array int | 是 | 人员系统编码 |
| NoComeRemark | string | 是 | 放鸽子备注 |
| NoComeType | int | 是 | 自定义枚举备注 |
| IsDove | int | 是 | 是否放鸽子 |




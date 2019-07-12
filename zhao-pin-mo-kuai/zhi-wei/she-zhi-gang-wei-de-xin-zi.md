# 设置岗位的客户可见薪资
##### _【功能说明】_ {#【功能说明】}

设置岗位的客户可见薪资


_**【应用场景】**_

设置岗位的客户可见薪资

_**【接口地址】**_

http://ip:port/RecruitAction/Position/SetPositionSalary

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionSysNo | int | 是 | 职位系统编码 |
| PositionSalaryList | array object | 否 | 客户可见岗位薪资列表 |
| Remark| string| 是 | 日志备注 |
| Reward|decimal| 否 | 平台奖励|
|Commission|decimal| 否 | 佣金|
|CommissionType|int| 否 | 佣金类型|










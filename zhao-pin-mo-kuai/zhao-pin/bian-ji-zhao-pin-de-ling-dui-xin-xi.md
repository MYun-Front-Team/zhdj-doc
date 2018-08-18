# 编辑招聘的领队信息

##### _【功能说明】_ {#【功能说明】}

编辑招聘的领队信息

_**【应用场景】**_

编辑招聘的领队信息



_**【接口地址】**_

http://ip:port/RecruitAction/Recruit/EditRecruit

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitSysNo | int | 是 | 招聘系统编码 |
| CustomerShopName| string| 是 | 客户名称 |
| CustomerSalary| decimal| 否 |客户薪资 |
| Commission| decimal| 否 |佣金 |
| Subsidy| decimal| 否 |补贴|
| CommissionType| int| 否 |佣金类型（不限制，端自定义） |
| PushLeaderEndTime| datetime| 否 |推送结束时间|
| SettlementType| int| 否 | 结算方式：1月结、2周结、3日结，4次日结，5完工结 |
| SettlementCycle| int| 否 | 结算周期 |
| CommissionRemark| string| 否 |佣金备注 |








#### _应答数据_ {#应答数据-}




# 编辑项目结算人员

##### _【功能说明】_ {#【功能说明】}
编辑项目结算人员

_**【应用场景】**_
编辑项目结算人员


_**【接口地址】**_

http://ip:port/RecruitAction/Settlement/EditSettlementItem

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SettlementItemSysNo | int | 是 | 项目结算系统编码 |
| WorkHour| int | 是 |工作小时数合计 |
| OvertimeHour| int | 是 |固定加班小时数 |
|GZOvertimeHour | int | 否 | 工作日加班时小时数 |
| GXOvertimeHour| int | 否 | 公休日加班时小时数 |
| Salary| decimal | 是 |时薪水 |
| SellerReward | decimal| 是 |商家奖励金|
| SellerFine| decimal| 是 |商家罚款|




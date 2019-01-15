# 获取结算人员详情
##### _【功能说明】_ {#【功能说明】}

获取结算人员详情

_**【应用场景】**_

获取结算人员详情

_**【接口地址】**_

http://ip:port/RecruitQuery/Settlement/GetSettlementItemBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SettlementItemSysNo | int | 是 | 项目结算人员系统编码 |




#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SettlementItemSysNo | int | 是 | 项目结算人员系统编码 |
| SettlementSysNo | int | 是 | 项目结算系统编码 |
| PersonSysNo| int | 是 | 人员系统编码 |
| RealName| string| 是 | 人员名称|
| CellPhoneNo| string| 是 | 手机号|
| OrganizationSysNo| int | 是 | 组织系统编码 |
| DataRangeSysNo| int | 是 |店铺数据范围结点编码 |
| ShopSysNo| int | 是 |店铺编码 |
| ShopName| string| 是 |店铺名称 |
| WorkHour| int | 是 |工作小时数合计 |
| OvertimeHour| int | 是 |固定加班小时数 |
| Salary| decimal | 是 |时薪水 |
| EntryDate| datetime| 是 |入职时间 |
| QuitDate| datetime| 是 |离职时间 |
| TotalAmount| decimal| 是 |应收薪资 |
| Remark| string| 是 |问题备注 |
| ItemStatus| int | 是 |状态（0初始，1已核对，10已发薪水，11平台退回，12员工退回） |
| EmployeeCheck| int | 是 |员工核对0初始，10核对|
| EmployeeBackStatus| int | 是 |员工退回（0初始，10已退回）|
| PlatformBackStatus| int | 是 |是否平台退回（0初始，10已退回）|
| FinishStatus| int | 是 |是否发薪水(0初始，10已发)|
# 获取项目结算人员列表
##### _【功能说明】_ {#【功能说明】}

获取项目结算人员列表

_**【应用场景】**_

获取项目结算人员列表

_**【接口地址】**_

http://ip:port/RecruitQuery/Settlement/GetSettlementItemList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StartSettlementDate|datetime | 否 | 开始考勤月份 |
| EndSettlementDate|datetime | 否 | 开始考勤月份 |
| PersonKeyWord| string| 是 | 人员关键字|
| ShopName| string| 是 |店铺名称 |
| ItemStatusList|array[int] | 是 |人员核对状态（0初始，1已核对，10已发薪水，11平台退回，12员工退回） |
| EmployeeCheckList| array[int] | 是 |员工核对0初始，10核对|
| EmployeeBackStatusList| array[int]| 是 |员工退回（0初始，10已退回）|
| PlatformBackStatusList| array[int]| 是 |是否平台退回（0初始，10已退回）|
| FinishStatusList| array[int] | 是 |是否发薪水(0初始，10已发)|
| SettlementSysNo | int | 是 | 项目结算系统编码 |
| PersonSysNo| int | 是 | 人员系统编码 |
| ShopSysNo| int| 是 |店铺编码 |



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
| DownSalary| decimal | 是 |下发薪水 |
| CardNo| string  | 是 | 银行卡号 |
| BankSysNo| int | 是 | 银行编码 |
| BankName| string  | 是 | 银行名称 |
| BankBranchName| string  | 是 | 支行名称 |
| IDCard| string  | 是 | 身份证号 |
| CheckCount| int | 是 |用户核对次数|
| PlatformAdjustCount| int | 是 |平台校对次数|
| ActualAmount| decimal| 是 |应发薪资|
| ColourType| int | 是 | 0正常 1红背景红文字 2红子|
| SellerReward | decimal| 是 |商家奖励金|
| SellerFine| decimal| 是 |商家罚款|

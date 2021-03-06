# 获取合同列表

##### _【功能说明】_ {#【功能说明】}

获取合同列表

_**【应用场景】**_

获取合同列表

_**【接口地址】**_

http://ip:port/RecruitQuery/Settlement/GetSettlementList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StartSettlementDate|datetime | 否 | 开始考勤月份 |
| EndSettlementDate|datetime |否 | 结束考勤月份 |
| OrganizationSysNo| int | 否 |所有者组织系统编码|
| SellerKeyWord| string| 否 |商家名称|
| TotalStatusList|array[int] | 否 | 状态（0草稿，1已提交，2考勤已发放（待员工核对）， 3部分员工核对，4全部员工核对（待回款），5已回款，11平台退回，12员工退回，9发放薪水中， 10已发薪水） |
| SubmitStatusList| array[int] | 否 |提交状态（0初始，10已提交）|
| SendStatusList| array[int] | 否|是否考勤发放（0初始，10已发放）|
| EmployeeBackStatusList| array[int] | 否|员工退回（0初始，10已退回）|
| PlatformBackStatusList| array[int] | 否 |是否平台退回（0初始，10已退回）|
| EmployeeCheckList| array[int] | 否 |员工核对0初始，1部分，10全部|
| MoneyBackList| array[int] | 否 |回款状态（0初始10正常回款11异常回款）|
| FinishStatusList| array[int] | 否 |是否发薪水(0初始，1发放薪水中 10已发)|
| SalesManagerPersonSysNo| int | 否 |销售经理系统编码| 


#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SettlementSysNo | int | 是 | 项目结算系统编码 |
| SettlementDate| datetime| 是 | 考勤月份开始 |
| SettlementDateEnd| datetime| 是 | 考勤月份结束 |
| OrganizationSysNo| int | 是 |所有者组织系统编码|
| SellerName| string| 是 |商家名称|
| SellerShortName| string| 是 |商家简称|
| ContractCode| string| 是 |商家合同号|
| SellerBossCellPhoneNo| int| 是 |商家老板手机号|
| ShopCount| int | 是 | 门店数 |
| WorkHour| int | 是 |工作小时数合计 |
| OvertimeHour| int | 是 | 固定加班小时数|
|GZOvertimeHour | int | 否 | 工作日加班时小时数 |
| GXOvertimeHour| int | 否 | 公休日加班时小时数 |
| ServiceCharge| decimal| 是 |服务费合计|
| TaxRate| decimal| 是 |税点|
| TotalAmount| decimal| 是 |开票金额|
| ActualAmount| decimal| 是 |实收金额|
| TotalStatus| int | 是 | 状态（0草稿，1已提交，2考勤已发放（待员工核对）， 3部分员工核对，4全部员工核对（待回款），5已回款，11平台退回，12员工退回，9发放薪水中，10已发薪水） |
| SubmitStatus| int| 是 |提交状态（0初始，10已提交）|
| SendStatus| int| 是 |是否考勤发放（0初始，10已发放）|
| EmployeeBackStatus| int| 是 |员工退回（0初始，10已退回）|
| PlatformBackStatus| int| 是 |是否平台退回（0初始，10已退回）|
| EmployeeCheck| int| 是 |员工核对0初始，1部分，10全部|
| MoneyBack| int| 是 |回款状态（0初始10正常回款11异常回款）|
| FinishStatus| int| 是 |是否发薪水(0初始，1发放薪水中，10已发)|
| MoneyBackRemark| string| 是 |实收金额备注|
| ColourType| int | 是 | 0正常 1红背景红文字 2红子|
| ItemActualAmount| decimal| 是 |应发薪资|


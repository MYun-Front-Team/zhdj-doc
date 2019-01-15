# 员工核对

##### _【功能说明】_ {#【功能说明】}
员工核对


_**【应用场景】**_
员工核对


_**【接口地址】**_

http://ip:port/RecruitAction/Settlement/CheckSettlement

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SettlementItemSysNo | int | 是 | 项目结算人员系统编码 |
| CheckStatus| int | 是 | 核对结果（10通过，11不通过） |
| Remark| string| 是 | 问题备注|

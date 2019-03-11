# 获取实名认证列表
##### _【功能说明】_ {#【功能说明】}

获取实名认证列表


_**【应用场景】**_

获取实名认证列表


_**【接口地址】**_

http://ip:port/RecruitQuery/Authentication/GetAuthenticationList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PlatAuditStatusList|array int | 是 | 平台核验状态（10审核通过，0待审核，11审核不通过） |
| StartCreateTime|datetime | 是 | 开始提交认证时间 |
| EndCreateTime|datetime | 是 | 结束提交认证时间 |
| KeyWord|string| 是 | 关键字 |


#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AuthenticationSysNo| int | 是 | 实名认证系统编码 |
| PersonSysNo| int | 是 | 人员编码 |
| RealName| string | 是 | 人员姓名 |
| CardNo| string  | 是 | 银行卡号 |
| BankSysNo| int | 是 | 银行编码 |
| BankName| string  | 是 | 银行名称 |
| BankBranchName| string  | 是 | 支行名称 |
| IDCard| string  | 是 | 身份证号 |
| OriginAddress| string  | 是 | 户籍地址|
| ContractAddress| string  | 是 |联系地址 |
| ZipCode| string  | 是 | 邮编|
| PlatAuditStatus| int | 是 | 平台核验状态（10审核通过，0待审核，11审核不通过） |
| PlatAuditRemark| string  | 是 |审核备注|
| PlatAuditTime| datetime  | 是 | 审核时间|
| CreateTime| string  | 是 |递交认证日期|
| FPersonIDCardUrl | string | 否 | 身份证正面 |
| BPersonIDCardUrl | string | 否 | 身份证反面 |
| FrontfileByte| string | 否 |身份证正面 |
| BackfileByte| string | 否 |身份证背面 |





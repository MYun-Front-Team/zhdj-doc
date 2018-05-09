# 获取银行卡列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取银行卡列表

_**【应用场景】**_

获取银行卡列表

_**【接口地址】**_

[http://ip:port/WalletQuery/Card/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)CardList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 是 | 来源系统编码 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CardSysNo | int | 是 | 银行卡系统编码 |
| CardType | int | 是 | 银行卡类型：0普通，1信用卡 |
| CardNo | string | 是 | 银行卡号 |
| CardName | string | 是 | 银行卡户名 |
| CardPhoneNo | string | 是 | 预留手机号 |
| Bank | object | 是 | 银行实体 |
| BankBranchName | string | 是 | 开户行-支行名称 |
| PCDCode | string | 否 | PCD编码 |
| PCDDescription | string | 否 | PCD详情 |
| AccountAddress | string | 否 | 开户行地址 |
| CardKey | string | 否 | 信用卡口令 |
| CardDate | string | 否 | 信用卡有效期 |
| IfVerifyCard| int | 是 | 是通过连接三方查证银行卡合法性 |
| IdentityNo| string | 是 | 银行卡预留身份证（验证合法性的话必传） |






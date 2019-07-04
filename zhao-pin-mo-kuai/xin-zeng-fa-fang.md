# 新增发放

##### _【功能说明】_ {#【功能说明】}

新增发放

_**【应用场景】**_

新增发放

_**【接口地址】**_

[http://ip:port/RecruitAction/Wallet/AddWage](http://ip:port/RecruitAction/Wallet/AddWage)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| WageItems | array\[WageItemAdd\] | 是 | 发放明细 |
| RecruitCertificateSysNo| int | 是 | 落地公司编码 |
| FileName| string| 是 | 文件名 |
| Remark| string| 否 | 备注 |


#### WageItemAdd

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RealName | string | 是 | 姓名 |
| IDCard | string | 是 | 身份正号 |
| CardNo | string | 是 | 银行卡 |
| WageAmount | decimal | 是 | 薪资 |
| CellPhoneNo | string | 是 | 手机号 |
| Remark | string | 是 | 备注 |
| Index | int | 是 | 行号 |
| SubAccountNo| string | 是 | 子账号|
| BankName| string| 是 | 银行名称 |


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HasError| bool| 是 | 是否成功 |
| Errors| array[AddWageErrorItem]| 是 | 是否成功 |

#### AddWageErrorItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RealName | string | 是 | 姓名 |
| IDCard | string | 是 | 身份正号 |
| CardNo | string | 是 | 银行卡 |
| WageAmount | decimal | 是 | 薪资 |
| CellPhoneNo | string | 是 | 手机号 |
| Remark | string | 是 | 备注 |
| Index | int | 是 | 行号 |
| SubAccountNo| string | 是 | 子账号|
| BankName| string| 是 | 银行名称 |
| ErrorMessage| string| 是 | 错误信息 |







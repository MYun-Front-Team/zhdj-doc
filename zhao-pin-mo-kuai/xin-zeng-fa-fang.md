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

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WageSysNo | int | 是 | 发放编码 |




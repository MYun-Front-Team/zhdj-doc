# 编辑薪资发放

##### _【功能说明】_ {#【功能说明】}

编辑薪资发放

_**【应用场景】**_

编辑薪资发放

_**【接口地址】**_

http://ip:port/RecruitAction/Wallet/EditWage

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WageSysNo | int | 是 | 发放编码 |
| WageItems | array[WageItemEdit] | 是 | 发放明细 |



#### WageItemEdit

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RealName | string | 是 |姓名|
| IDCard | string | 是 |身份正号|
| CardNo | string | 是 |银行卡|
| WageAmount |decimal | 是 |薪资|
| CellPhoneNo | string | 是 |手机号|
| Remark | string | 是 |备注|



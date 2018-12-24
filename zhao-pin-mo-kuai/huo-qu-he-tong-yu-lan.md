# 获取合同预览
##### _【功能说明】_ {#【功能说明】}

获取合同预览


_**【应用场景】**_

获取合同预览


_**【接口地址】**_

http://ip:port/RecruitQuery/Contract/GetCertificateViewUrl

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| dpi| string | 是 |预览图片清晰度，枚举值：96-低清（默认），120-普清，160-高清，240-超清|
| expireTime| string | 是 |链接有效期清|
| ThreePartyContractId| string | 是 |合同编号|
| PersonSysNo| int | 是 |人员系统编码|


#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| url| string | 是 | 预览地址 |



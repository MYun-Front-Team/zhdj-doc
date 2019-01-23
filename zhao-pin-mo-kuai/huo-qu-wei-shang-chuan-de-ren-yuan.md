#获取未上传的人员

##### _【功能说明】_ {#【功能说明】}

获取未上传的人员

_**【应用场景】**_
获取未上传的人员

_**【接口地址】**_

http://ip:port/RecruitQuery/Settlement/GetSettlementItemNoImportList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SettlementSysNo| int | 是 |结算系统编码|




#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RealName| string| 是 |姓名|
| CellPhoneNo| string| 是 |手机|

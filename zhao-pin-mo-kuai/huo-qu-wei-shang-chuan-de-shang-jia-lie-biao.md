#获取未/已经上传的商家列表

##### _【功能说明】_ {#【功能说明】}

获取未/已经上传的商家列表

_**【应用场景】**_

获取未/已经上传的商家列表

_**【接口地址】**_

http://ip:port/RecruitQuery/Settlement/GetUploadSellerList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StartSettlementDate|datetime | 否 | 开始考勤月份 |
| EndSettlementDate|datetime |否 | 结束考勤月份 |
| OrganizationSysNo| int | 否 |所有者组织系统编码|
| SellerKeyWord| string| 否 |商家名称|
| UploadStatus| int | 是 |10已上传，11未上传|




#### 返回参数

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SettlementDate| datetime| 是 | 考勤月份 |
| OrganizationSysNo| int | 是 |所有者组织系统编码|
| SellerName| string| 是 |商家名称|
| SellerShortName| string| 是 |商家简称|
| SellerBossCellPhoneNo| int| 是 |商家老板手机号|
| UploadStatus| int | 是 |10已上传，11未上传|
# 获取项目列表

##### _【功能说明】_ {#【功能说明】}

获取项目列表

_**【应用场景】**_

获取项目列表
_**【接口地址】**_

http://ip:port/ParkQuery/IndustryProject/GetParkProjectFollowList


> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProjectSysNo | int | 是 | 项目系统编码 |


> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FollowSysNo | int | 是 | 项目系统编码 |
| FollowDate | datetime | 否 | 跟进时间 |
| ProjectStatus | int | 否 | 项目状态（0潜在，1洽谈，2入住，3长期） |
| AgreementStatus | int | 否 | 协议状态（0未签署，10已签署） |
| FollowDesc | string | 否 | 跟进内容 |






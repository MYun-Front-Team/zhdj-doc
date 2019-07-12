# 设置领队激活状态
##### _【功能说明】_ {#【功能说明】}

设置领队激活状态


_**【应用场景】**_
设置领队激活状态



_**【接口地址】**_

http://ip:port/RecruitAction/Leader/SetLeaderActiveStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| LeaderSysNo| int| 是 |领队编码|
| ActiveStatus| int| 是 |激活状态(10已激活，11已禁用) |
| AuditRemark| string| 否 |审核备注|





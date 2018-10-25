# 获取沟通记录
##### _【功能说明】_ {#【功能说明】}

获取沟通记录


_**【应用场景】**_

获取沟通记录


_**【接口地址】**_

http://ip:port/RecruitQuery/Resume/GetCommunicateList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int |否 | 人员编码 |






#### 返回数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CommunicateSysNo | int | 是 | 系统编码 |
| CommunicateStatus| int | 是 |沟通状态（端定义）|
| Remark| string | 是 |沟通内容 |
| CreateTime| datetime| 是 |沟通时间|
| PersonFromName| string | 是 |沟通发起人 |















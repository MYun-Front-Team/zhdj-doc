# 添加沟通记录
##### _【功能说明】_ {#【功能说明】}

添加沟通记录


_**【应用场景】**_

添加沟通记录
T_Basic_PersonCommunicate表加记录

_**【接口地址】**_

http://ip:port/RecruitAction/Resume/AddCommunicate

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员编码 |
| CommunicateStatus| int | 是 |沟通状态（端定义）|
| Remark| string | 是 |沟通内容 |





#### 返回数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| | int | 否 | 系统编码 |









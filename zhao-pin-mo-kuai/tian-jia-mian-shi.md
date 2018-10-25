# 添加面试
##### _【功能说明】_ {#【功能说明】}

添加面试


_**【应用场景】**_
添加面试
T_Recruit_Interview表加记录

_**【接口地址】**_

http://ip:port/RecruitAction/Interview/AddInterview

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo| int| 是 |组织编码（先用平台组织）|
| DataRangeSysNo| int| 否 |数据范围结点编码|
| PositionSysNoList|array[int] | 是 | 岗位编码 |
| InterviewName| string| 是 |面试项目|
| StartTime| datetime| 是 |面试开始 |
| EndTime| datetime| 是 |面试结束|
| InterviewAddress| string| 是 |面试地址 |
| Longitude| decimal| 是 |经度|
| Latitude| decimal| 是 |维度|
| Remark| string| 否 |备注|





#### 返回数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| | int | 否 | 系统编码 |









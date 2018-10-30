# 添加面试
##### _【功能说明】_ {#【功能说明】}

添加面试


_**【应用场景】**_
添加面试
T_Recruit_Interview表加记录

PositionSysNoList几条就添加几个T_Recruit_Interview

_**【接口地址】**_

http://ip:port/RecruitAction/Interview/AddInterview

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionList|array[Position] | 是 | 岗位编码 |
| InterviewName| string| 是 |面试项目|
| StartTime| datetime| 是 |面试开始 |
| EndTime| datetime| 是 |面试结束|
| InterviewAddress| string| 是 |面试地址 |
| Longitude| decimal| 是 |经度|
| Latitude| decimal| 是 |维度|
| Remark| string| 否 |备注|


> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo|int | 是 | 组织编码 |
| DataRangeSysNo| int | 是 |数据结构树编码|
| ShopSysNo| int | 是 |店铺编码|
| PositionSysNo| int | 是 |岗位编码|
| RecruitSysNo| int| 否 |招聘编码|










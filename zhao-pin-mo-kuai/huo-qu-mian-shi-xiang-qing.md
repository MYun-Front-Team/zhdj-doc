# 获取面试详情
##### _【功能说明】_ {#【功能说明】}

获取面试详情


_**【应用场景】**_

获取面试详情


_**【接口地址】**_

http://ip:port/RecruitQuery/Interview/GetInterviewBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InterviewSysNo| int | 是 | 面试编码 |


#### Interview

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InterviewSysNo| int | 是 | 面试编码 |
| OrganizationSysNo | int |否| 组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围树枝叶编码列表 |
| ShopSysNo| int | 否 |店铺编码 |
| ShopName | string| 否 | 店铺 |
| SellerName| string| 否 | 商家名称|
| InterviewName| string| 是 |面试项目|
| StartTime| datetime| 是 |面试开始 |
| EndTime| datetime| 是 |面试结束|
| InterviewAddress| string| 是 |面试地址 |
| Longitude| decimal| 是 |经度|
| Latitude| decimal| 是 |维度|
| Remark| string| 否 |备注|
| Position| Position| 是 | 岗位列表 |
| InUser| string| 是 |创建人 |
| CreateTime| datetime| 是 |创建时间 |
| InterviewStatus| int | 是 |面试状态(0未开始 10进行中 11已结束)|









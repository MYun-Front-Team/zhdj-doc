# 获取面试列表
##### _【功能说明】_ {#【功能说明】}

获取面试列表


_**【应用场景】**_

获取面试列表


_**【接口地址】**_

http://ip:port/RecruitQuery/Interview/GetInterviewList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int |否| 组织系统编码 |
| DataRangeSysNoList | array[int] | 否 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord| string| 否 |关键字|
| InterviewShopSysNo| int | 否 | 商家店铺编码|
| InterviewOrganizationSysNo| int | 否 | 商家组织编码|
| PositionSysNo| int | 否 | 岗位编码|
| StartDate| datetime| 否 | 起始时间|
| EndDate| datetime| 否|终止时间|
| InterviewStatusList|array[int] | 否|面试状态(0未开始 10进行中 11已结束)|
| PersonSysNo| int | 否 |显示当前人的|

#### Interview

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InterviewSysNo| int | 是 | 面试编码 |
| InterviewName| string| 是 |面试项目|
| OrganizationSysNo | int |否| 组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围树枝叶编码列表 |
| ShopSysNo| int | 否 |店铺编码 |
| ShopName | string| 否 | 店铺 |
| SellerName| string| 否 | 商家名称|
| StartTime| datetime| 是 |面试开始 |
| EndTime| datetime| 是 |面试结束|
| InterviewAddress| string| 是 |面试地址 |
| Longitude| decimal| 是 |经度|
| Latitude| decimal| 是 |维度|
| Remark| string| 否 |备注|
| Position | Position| 是 | 岗位 |
| InUser| string| 是 |创建人 |
| CreateTime| datetime| 是 |创建时间 |
| InterviewStatus| int | 是 |面试状态(0未开始 10进行中 11已结束)|
| PersonStatus| int| 否 |面试人员状态（0邀约，10通过，11未通过）（显示当前人传了才有效） |
| ResultTime| datetime| 否 |面试结果时间（显示当前人传了才有效） |
| InvitePersonName| string| 否 |邀请人（显示当前人传了才有效） |
| InvitePersonCount| int| 否 |面试人数 |


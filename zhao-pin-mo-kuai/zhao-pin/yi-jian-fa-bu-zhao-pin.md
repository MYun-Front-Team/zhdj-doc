# 一键发布招聘 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

一键发布招聘

_**【应用场景】**_

一键发布招聘

注：1、发布需要圈子满足招聘要求的人员信息；

2、需要新增一条如7天到期之后的重复发布逻辑（Remind），并需要去掉忽略该条照片信息的人员；

_**【接口地址】**_

[http://ip:port/RecruitAction/Recruit/P](http://ip:port/HMAction/River/AddRiver)ublishRecruit

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitSysNo | int | 否 | 招聘系统编码（传了表示延长，不传表示新增） |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 否 | 所属数据范围树 |
| ShopSysNo | int | 否 | 店铺系统编码 |
| PositionSysNo | int | 是 | 职位编码 |
| StartDate | string | 否 | 开始时间 |
| EndDate | string | 否 | 结束时间 |
| PickRuleTemplateList | array object | 否（可选配置） | 选人规则 |
| IsAgent| int | 否 | 是否代理|




#### _应答数据_ {#应答数据-}




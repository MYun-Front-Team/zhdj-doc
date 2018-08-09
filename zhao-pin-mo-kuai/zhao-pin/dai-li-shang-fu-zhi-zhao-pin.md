# 代理商复制招聘
##### _【功能说明】_ {#【功能说明】}

代理商复制招聘


_**【应用场景】**_

代理商复制招聘


_**【接口地址】**_

http://ip:port/RecruitAction/Recruit/CopyRecruit

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 代理商组织系统编码 |
| DataRangeSysNo | int | 否 | 代理商所属数据范围树 |
| ShopSysNo | int | 否 | 代理商店铺系统编码 |
| RecruitSysNo | int | 是 | 模板招聘系统编码|
| RecruitCount | int | 是 | 招聘人数 |
| AgentRecruitShops| array RecruitShop | 否 |代理招聘的店铺组织 |
| IsAgent| int | 否 | 是否代理|



> #### RecruitShop

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 招聘商家组织系统编码 |
| DataRangeSysNo | int | 否 | 招聘商家所属数据范围树 |











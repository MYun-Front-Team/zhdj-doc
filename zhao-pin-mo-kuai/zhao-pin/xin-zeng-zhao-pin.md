# 代理新增招聘
##### _【功能说明】_ {#【功能说明】}

代理新增招聘


_**【应用场景】**_

代理新增招聘


_**【接口地址】**_

http://ip:port/RecruitAction/Recruit/AddRecruit

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 代理商组织系统编码 |
| DataRangeSysNo | int | 否 | 代理商所属数据范围树 |
| ShopSysNo | int | 否 | 代理商店铺系统编码 |
| PositionClassSysNo | int | 是 | 职位类型编码（分类） |
| PositionName | Nvarchar\(50\) | 是 | 职位名称（冗余） |
| PositionType | int | 否 | 工作类型:0不限,1全职,2兼职 |
| SexType | int | 否 | 性别要求：0不限,1男，2女 |
| RecruitCount | int | 否 | 招聘人数 |
| ExperienceRequirements | int | 否 | 经验要求：0不限,1一年内，2一到三年，3三到五年，4五到十年，5十年以上 |
| Remark | Nvarchar\(max\) | 否 | 备注 |
| PositionPathList | array string | 否 | 工作地Path文件列表 |
| PositionSalaryList | array object | 否 | 客户可见岗位薪资列表 |
| PositionAgeList | array object | 否 | 岗位年龄列表 |
| PositionWorkDayList | array object | 否 | 工作日期列表 |
| PositionWorkTimeList | array object | 否 | 工作时间列表 |
| TagClassList | array object | 否 | 福利标签列表（说明见通用） |
| CustomerPositionName| Nvarchar\(50\) | 否 | 客户自定义职位名称 |
| PositionDayAreaList | array object | 否 | 工作日期列表（日期） |
| AgentRecruitShops| array RecruitShop | 否 |代理招聘的店铺组织 |
| IsAgent| int | 否 | 是否代理|
| PlatPositionSalaryList | array object | 否 | 平台岗位薪资列表 |



> #### RecruitShop

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 招聘商家组织系统编码 |
| DataRangeSysNo | int | 否 | 招聘商家所属数据范围树 |





> #### _返回数据_ {#返回数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RecruitSysNo | int | 否 | 招聘系统编码（传了表示延长，不传表示新增） |








# 注册账号 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

注册账号

_**【应用场景】**_

注册账号

注：追加一个登录账号到指定的账户中。

场景1：PersonSysNo=0 and IsNewPerson = 0 默认可根据UserSysNo匹配到账户；

场景2：PersonSysNo &gt; 0 指定账户；

场景3：PersonSysNo=0 and IsNewPerson = 1 创建新人；

场景4：OrganizationSysNo&gt;0把该账号的人员关联到该组织；

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)AddLoginIn

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |
| PersonSysNo | int | 否 | 人员系统编码 |
| PersonName | string | 否 | 人员姓名昵称/真实姓名（当IsNewPerson=1时必填） |
| LoginSource | int | 是 | 登录来源（枚举） |
| LoginType | int | 是 | 登录类型（枚举） |
| LoginID | string | 是 | 用户名 |
| LoginPwd | string | 否 | 密码（微信等方式登录可为空） |
| IsEnable | int | 否 | 是否启用 |
| IsNewPerson | int | 否 | 是否新的人员（禁用） |
| OrganizationSysNo | int | 否 | 注册账号到指定的组织 |
| Post | string | 否 | 职位跟着人走 |
| AdminStatus | int | 否 | 状态：0未激活，1正常，2禁用 |
| WxUnionID | string | 否 | 微信UnionID |
| PostSysNo | int | 否 | 职位跟组织走\(HR、店长\)端自定义 |
| PCDDataRangeSysNoList | array\[int\] | 否 | 负责区域列表 |
| CellPhoneNo| string | 是 | 手机号（如果存在历史用户，就会合并用户，不存在就会新增） |
| IsDepartmentBoss | int | 否 | 是否部门领导|
| DepartmentSysNo| int | 否 | 部门|
| SourceType| int | 否 | 项目自定义来源（0默认，1销售，2交付，3运营等） |
| UserGender | int | 否 | 性别：1男，2女 |
| ContactTel| string | 是 | 联系方式（仅仅是备注，允许重复） |


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AdminSysNo | int | 是 | 账号编码 |
|  |  |  |  |




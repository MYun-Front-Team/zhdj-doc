# 获取账户详情 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取账户详情

_**【应用场景】**_

获取账户详情

_**【接口地址】**_

[http://ip:port/BasicQuery/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/G](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etUserBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |
| UserLimit | object | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| User | object | 是 | 账户实体对象 |

#### UserLimit说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowModule | int | 否 | 是否显示模块 |
| IsShowRole | int | 否 | 是否显示角色 |
| IsShowRight | int | 否 | 是否显示权限 |
| ModuleLimit | object | 否 | 模块限制条件，当显示模块=1时生效 |
| RoleLimit | object | 否 | 角色限制条件，当显示角色=1时生效 |
| RightLimit | object | 否 | 权限限制条件，当显示权限=1时生效 |

#### ModuleLimit说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowChildModule | int | 否 | 是否显示子模块 |
| IsShowRight | int | 否 | 是否显示权限 |
| RightLimit | object | 否 | 权限限制条件，当显示权限=1时生效 |

#### RoleLimit说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowRight | int | 否 | 是否显示权限 |
| RightLimit | object | 否 | 权限限制条件，当显示权限=1时生效 |

#### RightLimit说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowModule | int | 否 | 是否显示模块 |

#### User说明（详情） {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| UserSysNo | int | 是 | 账户系统编码（即AdminSysNo） |
| ActivationCode | string | 否 | 用户验证码：首次激活账户用 |
| AdminStatus | int | 是 | 状态：0未激活，1正常 |
| LastLoginDevice | string | 否 | 最后登录设备 |
| LastLoginDate | string | 否 | 上一次登录时间 |
| DeviceType | int | 否 | 设备类型：1IOS，2安卓，3小米，4华为 |
| DeviceToken | string | 否 | 设备Token |
| WxOpenID | string | 否 | 微信Openid |
| WxCorpUserID | string | 否 | 微信企业号用户ID |
| Remark | string | 否 | 备注 |
| ModuleList | array object | 否 | 模块列表 |
| RoleList | array object | 否 | 角色列表（见获取角色列表） |
| RightList | array object | 否 | 权限列表（见获取角色列表） |

#### Module说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块系统编码（枚举） |
| ModuleSourceType | int | 是 | 模块类型（枚举） |
| ModuleSourceClass | int | 否 | 模块分类（分类树） |
| ModuleName | string | 是 | 模块名称 |
| ModuleCode | string | 是 | 模块代码 |
| ChildModuleList | array object | 否 | 子模块列表 |
| RightList | array object | 否 | 权限列表（见获取角色列表） |




# 分润角色管理-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 否 | 组织系统编码（与业务模块无关联时，由分润角色生成） |
| ProfitRoleClassSysNo | int | 是 | 分润角色分类（通用） |
| ProfitRoleClassName | string | 是 | 分润角色分类名称 |
| ProfitRoleSysNo | int | 是 | 分润角色系统编码 |
| ProfitRoleName | string | 是 | 分润角色名称 |
| IsEnable | int | 是 | 是否有效：0无，1有 |
| Remark | string | 否 | 备注 |
| ModuleRelation | object | 否 | 模块关联 |
| Organization | object | 否 | 组织 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| KeyWord | string | 否 | 关键字搜索（名称） |
| IsEnableList | array int | 否 | 是否有效 |
| ProfitRoleClassSysNo | int | 否 | 分润角色分类 |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowOrganization | int | 否 | 是否显示组织 |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}




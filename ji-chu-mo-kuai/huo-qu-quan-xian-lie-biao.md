# 获取系统权限树 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取系统权限树

_**【应用场景】**_

获取系统权限树

注：根据项目标识符，先确认购买的模块，然后再获取权限并转换为树结构。

_**【接口地址】**_

[http://ip:port/BasicQuery/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)RightTree

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BizCompanyCode | int | 是 | 项目标识符（枚举） |
| DataRangeSysNo | int | 是 | 数据范围树编码 |

> #### _应答数据 （记录数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块系统编码 |
| ModuleName | string | 是 | 模块名称 |
| ModuleCode | string | 是 | 模块代码 |
| RightList | array list | 是 | 权限列表 |

#### RightList说明 {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RightSysNo | int | 是 | 权限系统编码 |
| RightName | string | 是 | 权限名称 |
| RightCode | string | 是 | 权限代码 |
| RightType | int | 是 | 权限类型：1模块，2子模块，3页面，4按钮 |
| ChildRightList | array list | 是 | 子权限列表（结构同） |




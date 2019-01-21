# 根据数据范围结点，获取组织人员列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

根据数据范围结点，获取组织人员列表

_**【应用场景】**_

根据数据范围结点，获取组织人员列表

注：按组织内部门先排序，部门内人员再排序；

_**【接口地址】**_

[http://ip:port/OrganizationQuery/Organization/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)OrganizationPersonList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 组织所属数据范围结点编码 |
| OrganizationSysNo | int | 否 | 组织系统编码 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| IsFather | int | 否 | 是否上一级：0否，1是 |
| keyWord | string | 否 | 关键字搜索（姓名） |
| Limit | object | 否 | 限制条件 |
| IsHasDepartment | int | 否 | 是否有部门 |
| DepartmentSysNo| int | 否 | 部门编码 |


> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Person | object | 是 | 人员实体 |
| Organization | object | 是 | 组织实体 |
| Department | object | 否 | 部门实体 |
| Post | object | 否 | 岗位实体 |
| User | object | 否 | 账户实体（见基本模块） |
| IsDepartmentBoss | int | 否 | 是否部门领导|




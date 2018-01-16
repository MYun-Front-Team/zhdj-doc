# 删除组织人员 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

删除组织人员

_**【应用场景】**_

删除组织人员

注：1、当Person存在多个组织时，则可直接删除与该组织的关系；

2、当Person只存在于即将删除的组织时，则需新增一个个人组织；

3、不允许删除个人组织的关系；

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/D](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)eleteOrgPerson

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| PersonSysNo | int | 是 | 人员系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




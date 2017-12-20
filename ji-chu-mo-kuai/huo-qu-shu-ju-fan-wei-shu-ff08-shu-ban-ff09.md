# 获取数据范围树（树版） {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取数据范围树

_**【应用场景】**_

树形结构，以数据权限来分割业务数据。

注：（OrganizationSysNo+DataRangeTreeType）和（TreeSysNo）二选一必填；

_**【接口地址】**_

[http://ip:port/BasicQuery/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)DataRangeTree2

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TreeSysNo | int | 是 | 树系统编码（枚举） |
| DataRangeSysNo | int | 否 | 枝叶系统编码（0则查询整棵树） |
| OrganizationSysNo | int | 否 | 组织系统编码 |
| DataRangeTreeType | int | 否 | 树类型（枚举） |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 系统编码 |
| DataRangeFatherSysNo | int | 是 | 父级系统编码 |
| DataRangeCode | string | 否 | 节点代码 |
| DataRangeName | string | 是 | 节点名称 |
| DataRangeTree | object | 是 | 子树结构对象 |
| IsEnable | int | 是 | 是否有效（应用场景是枝上面无权限，在下面的叶子有权限，那么不需要选中枝） |
| DataRangeGradeType | int | 是 | 节点等级：1省，2市，3区，4街道/县，5社区/村 |

注：DataRangeTree即为返回实体本身。


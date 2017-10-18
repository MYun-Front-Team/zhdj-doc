# 根据数据范围等级类型，获取数据范围列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

根据数据范围类型，获取数据范围列表

_**【应用场景】**_

根据数据范围类型，获取数据范围列表

_**【接口地址】**_

[http://ip:port/BasicQuery/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)DataRangeListByGradeType

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| TreeSysNo | int | 是 | 树系统编码（枚举） |
| DataRangeGradeType | int | 否 | 数据范围等级类型 |

> #### _应答数据 （返回结构同”获取数据范围树“，无子节点数据）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 系统编码 |
| DataRangeFatherSysNo | int | 是 | 父级系统编码 |
| DataRangeCode | string | 否 | 节点代码 |
| DataRangeName | string | 是 | 节点名称 |
| ~~DataRangeTree~~ | ~~object~~ | ~~是~~ | ~~子树结构对象~~ |
| IsEnable | int | 是 | 是否有效（应用场景是枝上面无权限，在下面的叶子有权限，那么不需要选中枝） |
| DataRangeGradeType | int | 是 | 节点等级：1省，2市，3区，4街道/县，5社区/村 |




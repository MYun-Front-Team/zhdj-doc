# 新增网格 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增网格

_**【应用场景】**_

新增网格

_**【接口地址】**_

[http://ip:port/ResidentAction/Grid/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddGrid

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 数据范围树枝叶编码 |
| GridName | string | 是 | 网格名称 |
| GridRange | string | 否 | 网格范围 |
| GridMaster | string | 否 | 负责人 |
| GridMasterTel | string | 否 | 负责人电话 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GridSysNo | int | 是 | 网格系统编码 |




# 获取行政区域列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取行政区域列表

_**【应用场景】**_

获取行政区域列表

_**【接口地址】**_

[http://ip:port/UMQuery/Area/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)AreaList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FatherAreaSysNo | int | 是 | 父级区域系统编码 |
| ShowFloorCount | int | 否 | 显示子集合层级数 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AreaSysNo | int | 是 | 系统编码 |
| AreaCode | string | 否 | 区域代码 |
| AreaName | string | 是 | 区域名称 |
| ChildAreas | object | 否 | 子集合 |




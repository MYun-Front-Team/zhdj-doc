# 新增网格员 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增网格员

_**【应用场景】**_

新增网格员

注：1、把某个人打上网格员的便签（表）并记录所在网格列表；

2、特殊情况是该人之前已经添加过，后来被设置为无效了，再次新增则重新设置为有效即可，并记录网格列表；

_**【接口地址】**_

[http://ip:port/ResidentAction/GridMan/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddGridMan

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员系统编码 |
| GridSysNoList | array int | 是 | 网格系统编码列表 |
| TagSysNoList | array int | 否 | 标签系统编码列表 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GridManSysNo | int | 是 | 系统编码 |




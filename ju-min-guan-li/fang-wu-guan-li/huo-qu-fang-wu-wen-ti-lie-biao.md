# 设置巡房状态 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

设置巡房状态

_**【应用场景】**_

设置巡房状态

注：1、GridManSysNo=0，则通过操作人User找到网格员；

2、巡房不能重复设置开始或者结束；

3、一旦巡房结束，需保持最近二次巡房的对照日志记录；

_**【接口地址】**_

[http://ip:port/ResidentAction/House/S](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etPatrolHouseStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HouseSysNo | int | 是 | 模块编码 |
| GridManSysNo | int | 否 | 网格员系统编码 |
| PatrolHouseStatus | int | 是 | 巡房状态：0开始，1结束 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




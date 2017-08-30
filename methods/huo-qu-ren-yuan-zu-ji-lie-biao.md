# 获取人员足迹列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取人员足迹列表

_**【应用场景】**_

获取人员足迹列表

_**【接口地址】**_

[http://ip:port/UMQuery/Info/GetInf](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)oPersonFootPrints

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InfoSysNo | int | 否 | 资讯系统编码 |
| SourceType | int | 否 | 足迹类型：0客户，1用户 |
| SourceSysNo | int | 否 | 对应系统编码 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

#### FootPrintList说明 {#应答数据-（巡河记录数组）}

（同资讯列表）


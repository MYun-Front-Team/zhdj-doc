# 新增党员荣誉 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增党员荣誉

_**【应用场景】**_

新增党员荣誉

_**【接口地址】**_

[http://ip:port/PartyAction/Honor/AddP](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)artyMemberHonor

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PartyMemberSysNo | int | 是 | 党员系统编码 |
| HonorTime | string | 是 | 荣誉获得日期 |
| HonorTitle | string | 是 | 荣誉抬头 |
| HonorContent | string | 是 | 荣誉说明 |
| Remark | string | 否 | 备注 |
| FilePathList | int | 否 | 文件或图片Path列表（第一张为首图） |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HonorSysNo | int | 是 | 荣誉系统编码 |

####  {#应答数据-（巡河记录数组）}




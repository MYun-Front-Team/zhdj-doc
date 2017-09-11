# 修改党员荣誉 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改党员荣誉

_**【应用场景】**_

修改党员荣誉

_**【接口地址】**_

[http://ip:port/PartyAction/Honor/EditP](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)artyMemberHonor

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HonorSysNo | int | 是 | 党员系统编码 |
| HonorTime | string | 否 | 荣誉获得日期 |
| HonorTitle | string | 否 | 荣誉抬头 |
| HonorContent | string | 否 | 荣誉说明 |
| Remark | string | 否 | 备注 |
| FilePathList | int | 否 | 文件或图片Path列表（第一张为首图） |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}




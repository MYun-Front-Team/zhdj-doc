# 修改党委支部 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改党委支部

_**【应用场景】**_

修改党委支部

_**【接口地址】**_

[http://ip:port/PartyAction/Party/EditP](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)artyBranch

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PartyBranchSysNo | int | 是 | 系统编码 |
| PartyBranchType | int | 否 | 党委支部类型: 1两新组织、2社区支部、3机关支部 |
| PartyBranchTime | string | 否 | 创建时间 |
| PartyBranchName | string | 否 | 名称 |
| PartyBranchShortName | string | 否 | 简称 |
| PartyBranchDuty | string | 否 | 党委支部职责 |
| PartyBranchTel | string | 否 | 党委支部联系电话 |
| PartyBranchDesc | string | 否 | 党委支部描述 |
| PartyBranchMaster | string | 否 | 负责人 |
| PartyBranchMasterPost | string | 否 | 负责人岗位 |
| PartyBranchPerson | string | 否 | 联系人 |
| PartyBranchPersonPhone | string | 否 | 联系人电话 |
| PartyBranchPersonPost | string | 否 | 联系人岗位 |
| Remark | string | 否 | 备注 |
| ContractAddress | string | 否 | 联系地址 |
| Longitude | decimal | 否 | 经度 |
| Latitude | decimal | 否 | 纬度 |
| PartyBranchStarCount | decimal | 否 | 星级 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}




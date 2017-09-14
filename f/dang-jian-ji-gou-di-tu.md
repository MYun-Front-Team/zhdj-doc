# 获取党委机构地图

##### _【功能说明】_ {#【功能说明】}

获取党委机构地图
_**【应用场景】**_

获取党委机构地图


_**【接口地址】**_

http://ip:port/PartyQuery/Party/GetPartyMap

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 查询条件 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 系统编码 |
| PartyBranchType | int | 是 | 党委支部类型: 1两新组织、2社区支部、3机关支部 |
| IsLeaf | int | 是 | 是否是叶子支部 |
| PartyBranchName | string | 是 | 党委支部名称 |
| PartyBranchDesc | string | 是 | 党委支部描述 |
| ChildrenCount | int | 是 | 孩子党委支部数|
| ContractAddress | string | 是 | 联系地图 |
| LeafInfos | array[PartyMapLeafInfo] | 是 | 叶子支部信息|
| MemberInfos | array[PartyMapMemberInfo] | 是 | 党员数量信息 |
| Longitude | string | 是 | 经度 |
| Latitude | string | 是 | 纬度 |
| Children | int | 是 | 孩子党委支部 |
| FlowMemberInfos | string | 是 | 流动党员数量信息 |
| PartyStations | array[PartyMapLeafInfo] | 是 | 党员先锋站点|






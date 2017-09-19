# 获取党支部人员地图

##### _【功能说明】_ {#【功能说明】}

获取党支部人员地图

_**【应用场景】**_

获取党委机构地图

_**【接口地址】**_

[http://ip:port/PartyQuery/Party/GetPartyMemberMap](http://ip:port/PartyQuery/Party/GetPartyMemberMap)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 查询条件 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 系统编码 |
| PartyBranchType | int | 是 | 党委支部类型: 1两新组织、2社区支部、3机关支部 |
| PartyBranchName | string | 是 | 党委支部名称 |
| PartyBranchDesc | string | 是 | 党委支部描述 |
| ContractAddress | string | 是 | 联系地图 |
| Longitude | decimal | 是 | 经度 |
| Latitude | decimal | 是 | 纬度 |
| FlowMemberInfos | array\[PartyMapMemberInfo\] | 是 | 流动党员数量信息 |
| MemberInfos | array\[PartyMapMemberInfo\] | 是 | 党员数量信息 |
| Items | array\[PartyMemberMapItem\] | 是 | 党员数量信息 |

### PartyMapMemberInfo

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Count | int | 是 | 数量 |
| InnerPartyStatus | int | 是 | 党内状态0积极份子，1预报党员，2正式党员 |

### PartyMemberMapItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PartyMemberSysNo | int | 是 | 党员编码 |
| FilePathList | array\[string\] | 是 | 头像地址 |
| FileUrlList | array\[string\] | 是 | 头像地址 |
| JoinPartyTime | string | 是 | 入党时间 |
| DataRangeSysNo | int | 是 | 所属支部 |
| CellPhoneNo | string | 是 | 联系方式 |
| RealName | string | 是 | 名字 |
| PersonSysNo | int | 是 | 人员编码 |
| InnerPartyStatus | int | 是 | 党内状态0积极分子，1预报党员，2正式党员 |
| Longitude | int | 是 | 经度 |
| Latitude | int | 是 | 纬度 |







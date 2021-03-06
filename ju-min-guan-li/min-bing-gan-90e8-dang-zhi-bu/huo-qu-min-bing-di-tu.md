# 获取民兵地图

##### _【功能说明】_ {#【功能说明】}

获取民兵地图

_**【应用场景】**_

获取民兵地图

_**【接口地址】**_

[http://ip:port/ResidentQuery/Resident/GetResidentSoldierMap](http://ip:port/ResidentQuery/Resident/GetResidentSoldierMap)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | array int | 否 | 数据范围树编码列表 |
| SoldierType | int | 否 | 民兵类型（1干部2党支部） |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeName | int | 是 | 数据范围树名称 |
| DataRangeSysNo | int | 是 | 数据范围树编码 |
| Longitude | decimal | 是 | 经度 |
| Latitude | decimal | 是 | 纬度 |
| Items | array\[Item\] | 是 | 人数信息 |

#### Item

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Post | int | 是 | 党内职务：10书记，20副书记，30组织委员，40宣传委员,50纪检委员，60工青妇委员,70组织员 ,90 统战委员; 干部职务：100营长，110营政治辅导员,120副营长，130营副政治辅导员，200连长，210连政治辅导员220副连长，230连副政治辅导员， |
| Count | int | 是 | 人员数量 |
| NameList | array\[string\] | 是 | 人员姓名列表 |




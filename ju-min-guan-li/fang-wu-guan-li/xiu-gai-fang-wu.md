# 修改房屋 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改房屋

_**【应用场景】**_

修改房屋

_**【接口地址】**_

[http://ip:port/ResidentAction/House/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditHouse

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HouseSysNo | int | 是 | 房屋系统编码 |
| DataRangeSysNo | int | 否 | 数据范围树枝叶编码 |
| GridSysNo | int | 否 | 网格系统编码 |
| GridManSysNoList | array int | 否 | 网格员系统编码列表 |
| ~~HouseMasterPerson~~ | ~~object~~ | ~~否~~ | ~~户主人员~~ |
| HouseNo | string | 否 | 房屋编号 |
| HouseName | string | 否 | 房屋名称 |
| HouseAddress | string | 否 | 房屋地址 |
| HouseArea | decimal\(18,2\) | 否 | 房屋面积 |
| HouseOrientation | string | 否 | 房屋朝向 |
| HouseFloorNum | int | 否 | 房屋楼层数 |
| HouseMemberNum | int | 否 | 家庭成员人数 |
| HousePathList | array string | 否 | 房屋图片路径列表 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




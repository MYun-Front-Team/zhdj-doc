# 房屋管理-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HouseSysNo | int | 是 | 系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树枝叶编码 |
| Grid | object | 否 | 网格（简） |
| GridManList | array object | 否 | 网格员列表（简） |
| HouseMasterPerson | object | 是 | 户主人员（简） |
| HouseNo | string | 否 | 房屋编号 |
| HouseName | string | 是 | 房屋名称 |
| HouseAddress | string | 否 | 房屋地址 |
| HouseArea | decimal\(18,2\) | 否 | 房屋面积 |
| HouseOrientation | string | 否 | 房屋朝向 |
| HouseFloorNum | int | 否 | 房屋楼层数 |
| HouseMemberNum | int | 否 | 家庭成员人数 |
| FatherDataRange | array object | 否 | 上级数据范围列表 |
| HousePathList | array string | 否 | 房屋图片路径列表 |
| HouseUrlList | array string | 否 | 房屋图片Url列表 |
| ~~RoomList~~ | ~~array object~~ | ~~否~~ | ~~房间列表~~ |
| PatrolHouseList | array object | 否 | 巡查记录列表 |
| TwoRoundElectrombile | int | 否 | 二轮电动车 |
| ThreeRoundElectrombile | int | 否 | 三轮电动车 |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RoomCount | int | 否 | 房间数量 |
| RoomPurposeStatistics | array object | 否 | 房间用途数量统计 |
| UnFinishedWorkCount | int | 否 | 待处理工单数量 |
| ElectrombileCount | int | 否 | 电动车总数 |

> #### RoomPurposeStatistics说明 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RoomPurpose | int | 否 | 房间用途：0自用，1出租 |
| Count | int | 否 | 数量 |

#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| HouseSysNo | int | 否 | 房屋系统编码 |
| GridSysNo | int | 否 | 网格系统编码 |
| GridManSysNo | int | 否 | 网格员系统编码 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| KeyWord | string | 否 | 关键字搜索（名称） |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowHouseUrlList | int | 否 | 是否显示房屋图片列表 |
| IsShowFatherDataRange | int | 否 | 是否显示父级列表（值N代表父级级别） |
| IsShowGrid | int | 否 | 是否显示网格 |
| IsShowGridManList | int | 否 | 是否显示网格员 |
| IsShowHouseMasterPerson | int | 否 | 是否显示户主 |
| ~~IsShowRoomList~~ | ~~int~~ | ~~否~~ | ~~是否显示房间列表~~ |
| IsShowRoomCount | int | 否 | 是否显示房间数量 |
| IsShowRoomPurposeStatistics | int | 否 | 是否显示房间用途数量统计 |
| IsShowPatrolCompareLogList | int | 否 | 是否显示对照类型日志列表 |
| IsShowPatrolHouseList | int | 否 | 显示最近巡查记录条数 |
| IsShowUnFinishedWorkCount | int | 否 | 是否显示待处理工单数 |




# 获取任务列表

获取任务列表

_**【应用场景】**_

获取任务列表
_**【接口地址】**_

http://ip:port/PointsQuery/LJPoint/GetMissionList



#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MissionSysNo| int | 是 | 任务系统编码 |
| MissionName| string | 是 | 任务名称 |
| MissionUrl| string | 是 | 任务跳转地址|
| MissionIcon| string | 是 | 任务图标|
| RewardMP| decimal| 是 | 奖励魔力|
| ModuleSysNo| int | 是 | 模块编码|
| ModuleSourceType| int | 是 | 模块类型|
| ModuleSourceClass| int | 是 | 分类编码|
| IsComplete| int | 是 | 是否完成|






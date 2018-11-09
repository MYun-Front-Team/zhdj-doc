# 获取冻结蓝晶/魔力列表

获取冻结蓝晶/魔力列表

_**【应用场景】**_

获取冻结蓝晶/魔力列表
_**【接口地址】**_

http://ip:port/PointsQuery/LJPoint/GetLJFrozenPoint




#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PointsType| int | 否 |积分类型（1蓝晶/2魔力） |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

#### Group {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PointsValue| decimal| 是 | 当前魔力/蓝晶|
| PointsType| int | 否 |积分类型（1蓝晶/2魔力） |
| Remark| string | 是 | 冻结备注 |
| DateTime| datetime| 是 | 冻结时间 |
| ModuleFromSysNo| int| 是 | 模块编码 |
| ModuleSourceType| int| 是 | 模块类型 |
| ModuleSourceClass| int| 是 | 模块类别 |
| ModuleSourceSysNo| int| 是 | 来源编码|










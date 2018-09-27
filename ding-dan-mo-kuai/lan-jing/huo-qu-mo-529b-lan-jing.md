# 获取商品列表

获取商品列表

_**【应用场景】**_

获取商品列表

_**【接口地址】**_

http://ip:port/PointQuery/LJPoint/GetLJPoint

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PointsType| int | 否 |积分类型（1蓝晶/2魔力） |



> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Total| Total| 是 | 魔力/蓝晶汇总|
| Items|array[Item]| 是 | 魔力/蓝晶明细 |



#### Total

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PointsValue| decimal| 是 | 当前魔力/蓝晶|
| AvaPointsValue| decimal| 是 | 可用魔力/蓝晶|
| FroPointsValue| decimal| 是 | 冻结魔力/蓝晶|
| HisPointsValue| decimal| 是 | 历史魔力/蓝晶|
| UncPointsValue| decimal| 是 | 不可兑换魔力/蓝晶|




#### Item

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ChangePointsValue| decimal| 是 | 魔力/蓝晶（正数/负数）|
| Remark| string| 是 | 备注|
| CreateTime| datetime| 是 |创建时间|



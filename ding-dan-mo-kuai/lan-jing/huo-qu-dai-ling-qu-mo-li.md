# 获取待领取魔力/蓝晶

获取待领取魔力/蓝晶

_**【应用场景】**_

获取待领取魔力/蓝晶

_**【接口地址】**_

http://ip:port/PointsQuery/LJPoint/GetPickLJPoints

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PointsType| int | 否 |积分类型（1蓝晶/2魔力） |
| PersonSysNo| int | 否 |人员系统编码 |


#### 返回

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PickLJPointSysNo| int| 是 | 系统编码|
| PointsType| int | 否 |积分类型（1蓝晶/2魔力） |
| PointsValue| decimal| 是 | 分数|




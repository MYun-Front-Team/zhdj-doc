# 获取魔力/蓝晶排行榜

获取魔力/蓝晶排行榜

_**【应用场景】**_

获取魔力/蓝晶排行榜

_**【接口地址】**_

http://ip:port/PointsQuery/LJPoint/GetLJPointRank

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PointsType| int | 否 |积分类型（1蓝晶/2魔力） |



> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonName | string| 是 | 买家人员昵称 |
| PointsValue| decimal| 是 | 当前魔力/蓝晶|
| FileUrlList | array string | 否 | 头像图片列表 |






# 获取楼层列表

##### _【功能说明】_ {#【功能说明】}

获取楼层列表

_**【应用场景】**_

获取楼层列表

_**【接口地址】**_

http://ip:port/ResidentQuery/Floor/GetFloorList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Query | object | 是 | 见搜索条件 |
| Limit | array | 否 | 限制条件 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FloorBase | object | 是 | 基础字段 |
| FloorStatistic | object | 否 | 统计字段 |




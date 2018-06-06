# 获取房间使用率

##### _【功能说明】_ {#【功能说明】}

获取房间使用率

_**【应用场景】**_

获取房间使用率

_**【接口地址】**_

http://ip:port/ParkQuery/IndustryPark/GetParkRoomRentRate


> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Query | object | 是 | 见搜索条件 |
| Limit | array | 否 | 限制条件 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Items|array [ParkRoomRentRate] | 是 |占用/非占用统计 |

#### ParkRoomRentRate

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsRent | int | 是 | 租借状态(0闲置 10租用) |
| Count| int| 是 | 数量|
| Rate| decimal| 是 | 比率（没有乘100）|







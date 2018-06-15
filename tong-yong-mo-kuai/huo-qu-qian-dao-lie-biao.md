# 获取签到列表

##### _【功能说明】_ {#【功能说明】}

获取签到列表

_**【应用场景】**_

获取签到列表

_**【接口地址】**_

http://ip:port/UMQuery/Sign/GetSignList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 否 | 人员编码 |
| StartDate | datetime | 否 | 开始时间 |
| EndDate | datetime | 否 | 开始时间 |




> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SignItems | array[SignItem] | 否 | 签到明细|
| SignDay | int | 否 | 连续签到天数 |

#### SignItem

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SignDate | datetime | 否 | 开始时间|
| Longitude| decimal| 否 | Longitude |
| Latitude| decimal| 否 | Latitude |



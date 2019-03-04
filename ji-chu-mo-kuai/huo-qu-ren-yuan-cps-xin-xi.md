#获取人员CPS信息列表



##### _【功能说明】_ {#【功能说明】}

获取人员CPS信息列表

_**【应用场景】**_

获取人员CPS信息列表



_**【接口地址】**_

http://ip:port/BasicQuery/Basic/GetCPSPositionList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 否 | 人员编码 |


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ChannelId| string  | 否 | 栏目ID|
| MemberId | string | 否 | 会员ID |
| CPSCode | string | 否 |CPS编码 |
| CPSSysNo| int| 否 |CPS系统编码 |
| PositionId| string| 否 |推广位编码|
| WebId| string| 否 |推广网站编码|
| APPId| string| 否 |推广app编码|

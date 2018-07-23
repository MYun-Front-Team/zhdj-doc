# 获取企业租赁房间汇总

##### _【功能说明】_ {#【功能说明】}
获取企业租赁房间汇总
_**【应用场景】**_

获取企业租赁房间汇总

_**【接口地址】**_

http://ip:port/ParkQuery/IndustrySale/GetParkRoomRentTotal

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 企业组织系统编码 |
| IfShowRent| int | 否 | 是否只显示当前租的|
| ParkRoomSysNo| int | 否 | 房间编码|


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BuildingArea| decimal | 否 |总建筑面积|




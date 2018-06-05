# 新增待收费查询

##### _【功能说明】_ {#【功能说明】}

新增待收费查询（只对房租和物业费有效）

_**【应用场景】**_

新增待收费查询（只对房租和物业费有效）



_**【接口地址】**_

http://ip:port/ParkQuery/IndustryFee/GetWaitPayFee



> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FeeType | int | 是 | 费用类型 |
| EndDate | datetime | 是 | 费用结束时间 |
| ParkFloorSysNo | int | 否 | 楼层编码 |
| ParkSysNo | int | 否 | 园区编码 |
| BuildingSysNo | int | 否 | 楼宇编码 |
| OrganizationSysNo | int | 是 | 企业组织系统编码 |
|ParkRoomType | int | 否 |房间类型|




> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ParkFloorSysNo | int | 否 | 楼层编码 |
| ParkSysNo | int | 否 | 园区编码 |
| BuildingSysNo | int | 否 | 楼宇编码 |
| ParkRoomSysNo | int | 是 | 房间系统编码 |
| OrganizationSysNo | int | 是 | 企业组织系统编码 |
| ParkName | string | 否 | 园区名称 |
| ParkRoomName| int | 否 | 房间名称|
| ParkFloorName | string | 否 | 楼层名称 |












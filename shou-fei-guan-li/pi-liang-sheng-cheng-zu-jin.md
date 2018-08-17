# 批量生成租金

##### _【功能说明】_ {#【功能说明】}

批量生成租金

_**【应用场景】**_

批量生成租金

_**【接口地址】**_

[http://ip:port/ParkAction/IndustryFee/VolumeFee](http://ip:port/ParkQuery/IndustryFee/GetWaitPayFee)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StartDate | datetime | 是 | 收费开始时间 |
| EndDate | datetime | 是 | 收费结束时间 |
| ParkFloorSysNo | int | 否 | 楼层编码 |
| ParkSysNo | int | 否 | 园区编码 |
| BuildingSysNo | int | 否 | 楼宇编码 |
| ParkRoomTypeList | int | 否 | 房间类型 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 




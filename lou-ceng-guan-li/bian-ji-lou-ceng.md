#编辑楼层

##### _【功能说明】_ {#【功能说明】}

编辑楼层

_**【应用场景】**_

编辑楼层

_**【接口地址】**_

http://ip:port/ParkAction/IndustryPark/EditParkFloor

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ParkFloorSysNo | int | 是 | 楼层编码 |
| BuildingSysNo | int | 否 | 楼宇编码 |
| ParkFloorType | int | 否|楼层类型|
| ParkFloorClassSysNo | int | 否 | 楼层分类（枚举） |
| ParkFloorName | string | 否 | 楼层名称 |
| ParkFloorArea| decimal | 否 | 楼层面积|
| Remark | string | 否 | 楼层备注 |
| FilePathList | array string | 否 |照片 |



> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| BuildingSysNo | int | 是 | 楼宇系统编码 |



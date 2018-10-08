# 获取房屋报表

##### _【功能说明】_ {#【功能说明】}

获取房屋列表

_**【应用场景】**_

获取房屋列表

_**【接口地址】**_

http://ip:port/ResidentQuery/House/GetHouseReport



> #### 请求数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |




> #### 应答数据 

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HouseMasterPersonName| string | 是 | 户主姓名|
| DataRanges| array[DataRange]| 是 | 省-市-区……|
| HouseAddress| string| 是 | 详细地址|
| HouseMasterCellPhoneNo| string| 是 | 户主手机号|
| Floors| array[Floor]| 是 | 楼层信息|
| Rooms| array[Room]| 是 | 房间信息|














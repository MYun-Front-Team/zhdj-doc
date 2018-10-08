# 居民报表

#### 页面编号枚举说明 {#请求数据}

| 页编码 | 模块说明 | 页面说明 |
| :--- | :--- | :--- |
| 25004100 | 居民报表按房屋| 居民报表按房屋 |




> #### 请求数据（PageRequestData）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | int | 是 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |




> #### 应答数据 （PageResponseBase）【25004100】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HouseMasterPersonName| string | 是 | 户主姓名|
| DataRanges| array[DataRange]| 是 | 省-市-区……|
| HouseAddress| string| 是 | 详细地址|
| HouseMasterCellPhoneNo| string| 是 | 户主手机号|
| Floors| array[Floor]| 是 | 楼层信息|



#### Floor

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FloorName| string| 是 | 楼层信息|
















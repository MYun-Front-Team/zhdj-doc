# 获取坐标，获取区域 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取坐标，获取区域

_**【应用场景】**_

获取坐标，获取区域

注：通过经纬度，调用EDI获取PCD详情，在根据区域代码匹配系统的记录。

_**【接口地址】**_

[http://ip:port/UMQuery/Area/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)AreaByPoint

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Longitude | decimal\(18,10\) | 是 | 经度 |
| Latitude | decimal\(18,10\) | 是 | 纬度 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AreaSysNo | int | 是 | 区域系统编码 |
| AreaCode | string | 是 | 区域代码 |
| AreaName | string | 是 | 区域名称 |




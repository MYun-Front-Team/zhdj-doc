# 获取店铺开店状态（详情） {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取店铺开店状态

_**【应用场景】**_

获取店铺开店状态

注：通过设备找店铺，然后返回店铺的状态；

_**【接口地址】**_

[http://ip:port/ShopQuery/Shop/Get](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ShopOpenStatusBySysNo2

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ~~ShopSysNo~~ | ~~int~~ | ~~是~~ | ~~店铺系统编码~~ |
| DeviceSysNo | int | 是 | 设备系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OpenStatus | int | 是 | 开店状态：10开，11关（状态来源启用关系表） |
| OpenPerson | object | 否 | 开店人员（组织来源店铺的组织） |




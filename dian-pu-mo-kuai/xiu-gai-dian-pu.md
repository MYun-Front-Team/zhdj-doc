# 修改店铺 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改店铺

_**【应用场景】**_

修改店铺

_**【接口地址】**_

[http://ip:port/ShopAction/Shop/EditShop](http://ip:port/OrganizationAction/Customer/AddCustomer)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ShopSysNo | int | 是 | 组织系统编码 |
| ShopName | string | 否 | 店铺名称 |
| ShopShortName | string | 否 | 店铺简称 |
| ShopTel | string | 否 | 店铺联系电话 |
| ShopDesc | string | 否 | 店铺描述 |
| ShopMaster | string | 否 | 店铺负责人 |
| ShopPost | string | 否 | 店铺负责人岗位 |
| ShopPerson | string | 否 | 店铺联系人 |
| ShopPersonPhone | string | 否 | 店铺联系人电话 |
| ShopPersonPost | string | 否 | 店铺联系人岗位 |
| ContractAddress | string | 否 | 联系地址 |
| Longitude | decimal（18，10） | 否 | 经度 |
| Latitude | decimal（18，10） | 否 | 纬度 |
| OpenStatus | int | 否 | 开店状态：0开，1关 |
| OpenTime | string | 否 | 开店时间 |
| BusinessStartTime | string | 否 | 营业开始时间 |
| BusinessEndTime | string | 否 | 营业结束时间 |
| ServiceStartTime | string | 否 | 客服服务开始时间 |
| ServiceEndTime | string | 否 | 客服服务结束时间 |
| ShopLogoPathList | array string | 否 | 店铺Logo的Path路径列表 |

#### _应答数据 _ {#应答数据-}




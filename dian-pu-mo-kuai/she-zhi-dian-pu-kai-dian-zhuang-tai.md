# 设置店铺开店状态

##### _【功能说明】_ {#【功能说明】}

设置店铺开店状态

_**【应用场景】**_

设置店铺开店状态

_**【接口地址】**_

http://ip:port/ShopAction/Shop/SetShopOpenStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ShopSysNo | int | 是 | 店铺系统编码（当DeviceSysNo=0时必填） |
| OpenStatus | int | 是 | 开店状态：0初始，10开，11关 |
| Reamrk| string| 是 | 禁用备注|




#### _应答数据 _ {#应答数据-}




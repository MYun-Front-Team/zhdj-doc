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
| OpenStatus | int | 否 | 开店状态 |
| OpenTime | string | 否 | 开店时间 |
| BusinessStartTime | string | 否 | 营业开始时间 |
| BusinessEndTime | string | 否 | 营业结束时间 |
| ServiceStartTime | string | 否 | 客服服务开始时间 |
| ServiceEndTime | string | 否 | 客服服务结束时间 |
| ShopLogoPathList | array string | 否 | 店铺Logo的Path路径列表 |
| ShopNo | string | 否 | 店铺编号 |
| ShopUsedStatus | int | 否 | 店铺使用状态：0闲置，10使用 |
| ShopArea | decimal（18，2） | 否 | 店铺面积（平方） |
| ShopPropertyFee | decimal（18，2） | 否 | 店铺物业费（元/年） |
| ShopDepositFee | decimal（18，2） | 否 | 店铺默认押金（元） |
| ShopRentFee | decimal（18，2） | 否 | 店铺默认租金（元/月） |
| ShopRentRemark | string | 否 | 备注 |
| CategorySysNoList | int | 否 | 主营分类系统编码列表 |
| BrandSysNo | int | 否 | 品牌系统编码 |
| ShopCommission | decimal（18，4） | 否 | 店铺佣金 |
| RmaAddress | string | 否 | 退货地址 |
| ShopBannerPathList | array string | 否 | 店铺Banner图片列表 |
| SortNo | int | 否 | 排序 |
| ShopShowSourceSysNos|array[int] | 否 | 店铺展示位置 |
| IsScanCode| int | 否 | 是否有扫码功能 |
| RecruitNeedAudit| int | 否 |发布岗位是否要审核（1要，0不要） |
| IsAuthentication| int | 否 | 是否认证 |
| PositionPathList | array string | 否 | 工作地Path文件列表 |
| ShopPersonSysNo | int  | 否 | 店铺负责人编码（店长） |
| ------- | -以下为11-12抢班- | -- | ------- |
| ShopInterviewDateList | array ShopInterviewDateEdit | 否 | 面试时间 |



#### _应答数据 _ {#应答数据-}

#### ShopInterviewDateEdit

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ShopInterviewDateSysNo| int| 是 |面试时间系统编码|
| StartDate| datetime| 是 |开始面试时间（只有时分秒有效）|
| EndDate| datetime| 是 |结束面试时间（只有时分秒有效） |



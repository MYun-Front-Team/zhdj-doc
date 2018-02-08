# 优惠券管理-字段说明 {#新增河流}

> #### 基础字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CouponSysNo | int | 是 | 优惠券系统编码 |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| ShopSysNo | int | 是 | 店铺编码 |
| CouponType | int | 是 | 类型，1001-免邮，1002-全场通用，1003-限定商品，1004-满件券 |
| CouponSubType | int | 是 | 优惠券子类型，0-总金额满减，1-单件金额满减 |
| CouponName | string | 是 | 优惠券名称 |
| Description | string | 否 | 说明描述 |
| FullAmount | decimal\(18,2\) | 否 | 需满金额 |
| FullQuantity | int | 否 | 需满件数 |
| ReduceAmount | decimal\(18,2\) | 是 | 减少金额 |
| ReduceLimit | decimal\(18,2\) | 否 | 减免上限 |
| CouponDateType | int | 是 | 时间类型：0时间段，1天数 |
| StartDate | string | 是 | 优惠券开始时间 |
| EndDate | string | 是 | 优惠券结束时间 |
| CouponDays | int | 是 | 使用天数（当时间类型为1） |
| TotalNumber | int | 是 | 优惠券总量 |
| PerLimit | int | 是 | 每个人限领数量：0不限制 |
| DispatchType | int | 是 | 发放类型，0-通用，1-自领，2-后台发放 |
| PickUpStartDate | string | 否 | 领取开始时间 |
| PickUpEndDate | string | 否 | 领取结束时间 |
| CouponStatus | int | 是 | 状态：0新建,10发布,11撤下 |
| OverlayType | int | 是 | 叠加类型，0-不可叠加，1-可叠加 |
| IsShareToPublic | int | 是 | 是否分享：0否，1是 |
| IsSendToFriend | int | 是 | 是否转增：0否，1是 |
| IsUnifiedCoding | int | 是 | 是否统一编码：0否，1是 |
| TicketCode | string | 否 | 券编码\(当统一编码=1必填\) |
| IsReturn | int | 是 | 是否返还：0否，1是 |
| Organization | object | 否 | 组织 |
| Shop | object | 否 | 店铺 |
| Seller | object | 否 | 商家 |
| ~~CategorySysNoList~~ | ~~array int~~ | ~~否~~ | ~~商品分类系统编码列表~~ |
| ~~CustomerLevelSysNoList~~ | ~~array int~~ | ~~否~~ | ~~客户等级系统编码列表~~ |

> #### 统计计算字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsOverDue | int | 是 | 是否过期：0否，1是 |
| SendedCount | int | 否 | 已发数量 |
| UsedCount | int | 否 | 已使用数量 |

> #### 功能按钮字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |


#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CouponSysNo | int | 否 | 优惠券系统编码 |
| OrganizationSysNo | int | 否 | 所有者组织系统编码 |
| ShopSysNo | int | 否 | 店铺系统编码 |
| CouponTypeList | array int | 否 | 类型，1001-免邮，1002-全场通用，1003-限定商品，1004-满件券 |
| KeyWord | string | 否 | 关键字搜索（名称） |
| CouponStatusList | array int | 否 | 状态：0新建,10发布,11撤下 |
| CouponCode | string | 否 | 优惠券代码 |

> #### 查询Limit字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowOrganization | int | 否 | 是否显示组织 |
| IsShowShop | int | 否 | 是否显示店铺 |
| IsShowSeller | int | 否 | 是否显示商家 |
| IsShowSendedCount | int | 否 | 是否显示已发数量 |
| IsShowUsedCount | int | 否 | 是否显示已使用数量 |

####  {#应答数据-（巡河记录数组）}

#### 模块页面编号枚举说明 {#请求数据}




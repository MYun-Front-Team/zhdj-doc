# 修改款 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改款

_**【应用场景】**_

修改款

注：只能修改属于自己数据范围结点内且IsCreator=1的商品；

_**【接口地址】**_

[http://ip:port/ProductAction/](http://ip:port/HMAction/River/AddRiver)[P](http://ip:port/HMAction/River/AddRiver)roductGroup[/E](http://ip:port/HMAction/River/AddRiver)ditProductGroup

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ~~DataRangeSysNoList~~ | ~~array int~~ | ~~是~~ | ~~数据范围枝叶编码列表（必须在不同的树中的枝叶）~~ |
| ProductGroupSysNo | int | 是 | 款号系统编码 |
| ProductClassSysNo | int | 否 | 类型分类系统编码（类别树） |
| IndustryClassSysNo | int | 否 | 类型分类系统编码（行业树） |
| ProductGroupName | string | 否 | 款名称 |
| ProductGroupDetail | string | 否 | 详情 |
| ProductGroupMemo | string | 否 | 备注 |
| PCDCode | string | 否 | 产地PCD代码 |
| PCDDescription | string | 否 | 产地PCD描述 |
| GoodsWeight | decimal\(18,2\) | 否 | 重量 |
| GoodsVolumn | decimal\(18,2\) | 否 | 体积 |
| UnitSysNoList | array int | 否 | 计量单位系统编码列表 |
| SpecGroup | object | 否 | 规格组（说明见”获取规格模板列表“） |
| EditSkuList | array object | 否 | 修改规格列表（说明见”新增款规格“） |
| TagSysNoList | array int | 否 | 标签列表 |
| BrandSysNoList | array int | 否 | 品牌列表 |
| SupplierSysNoList | array int | 否 | 供应商列表 |
| ProductServiceType | int | 否 | 服务方式：0物流配送，1到店消费 |
| IsDisableRMA | int | 否 | 是否禁用退货：0否，1是 |
| CommissionRate | decimal（18，4） | 否 | 佣金比例 |
| EffectiveType | int | 否 | 有效类型：0天数，1日期 |
| EffectiveDays | int | 否 | 有效天数 |
| EffectiveDate | string | 否 | 有效期 |
|IsHidden|int | 否 | 是否隐藏 |
| IsSupportPointPay| int | 否 | 是否支持积分支付 |
| RewardPoint| int | 否 | 奖励积分 |
| ServiceType| int | 否 | 消费方式（0按次数，1按时间） |
| ServiceOutMinutes| int | 否 | 过期时间（分钟）（0为长期有效）|
| GroupSysNos| Array[int]| 否 |商品分组|
| CPSCategory| string| 否 |三方CPS类别 |
| CPSMaterialUrl| string| 否 |三方CPSURL |
| CPSStartDate| string| 否 |三方CPS开始推荐 |
| CPSEndDate| string| 否 |三方CPS结束推荐 |
| CPSInOrderCount| int | 否 |三方CPS评价 |
| FakeInventoryCount| int | 否 |可砍份数 |
| RewardMP| decimal| 否 | 奖励魔力|
| FakeSaleCount|int| 否 |虚假销量|
| CPSMaterialUrl|string| 否|CPS落地页|
| CPSSysNo | int | 否 | CPS编码 |
| SourceCPSSysNo|int| 是 |来源三方CPS|
| CPSStartDate | string | 否 | 三方CPS开始推荐 |
| CPSEndDate | string | 否 | 三方CPS结束推荐 |
| SourceProductGroupCode|string| 是 |来源三方编码|
| TaoWord|string| 是 |淘口令|
| StartSaleDate| datetime| 是 | 开卖时间|
| GroupByCode| string| 否 | 多款聚合规格名称 |
| IsGroupByDefault| int | 否 | 多款聚合默认显示 |
| GroupByOtherName| string| 否 | 多款聚合别名 |
| ShopShowSourceList|array[int] | 否 |展示来源（0普通，1蓝晶兑换） |
| SubsidyMP | decimal | 否 | 补贴魔力 |
| SubsidyMPRate | decimal | 否 | 补贴魔力比率 |
| LimitBuyCount | int | 否 | 限购数|
| IsAllSubsidyMP | int | 否 | 无论商品购买多少个，补贴魔力只给1份|
| LimitSubsidyMPStart | datetime | 否 | 限购魔力锁开始时间|
| LimitSubsidyMPEnd | datetime | 否 | 限购魔力锁结束时间|
| LimitSubsidyMPCount | int | 否 | 限购魔力锁最大份数|
| IsLockOnSaleStatus | int | 否 | 是否锁定上下架状态 |
| SubsidyMPLimitNewPerson | int | 否 | 补贴魔力是否只给新人（1是 0否）|
| BasicCommissionRate| decimal\(18,2\) | 否 |自购佣金比例 |
| Properties| string| 否 | 商品属性（Json字符串） |
| OnSaleStatus | int | 是 | 上下状态:0待上架 1上架 2下架 3部分上架 4停售 |
| IsLockBasicCommissionRate| decimal\(18,2\) | 否 |是否锁定自购佣金比例 |






#### _应答数据_ {#应答数据-}




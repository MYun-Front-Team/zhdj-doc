# 新增款 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增款

_**【应用场景】**_

新增款

注：调用该接口说明该商品属于该组织，IsCreator=1；

注：DataRangeSysNo为空时，找到该组织的默认店铺编码；

注：ProductGroupCode为空时的自动生产规则：数据范围结点+至少3位长度的商品数量；

_**【接口地址】**_

[http://ip:port/ProductAction/](http://ip:port/HMAction/River/AddRiver)[P](http://ip:port/HMAction/River/AddRiver)roductGroup[/Add](http://ip:port/HMAction/River/AddRiver)ProductGroup

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| DataRangeSysNo | int | 否 | 数据范围枝叶编码 |
| ProductType | int | 是 | 类型（枚举） |
| ProductClassSysNo | int | 否（可选配置） | 类型分类系统编码（类别树） |
| IndustryClassSysNo | int | 否（可选配置） | 类型分类系统编码（行业树） |
| ProductGroupCode | string | 否（可选配置） | 款号 |
| ProductGroupName | string | 是 | 款名称 |
| ProductGroupDetail | string | 否（可选配置） | 详情 |
| ProductGroupMemo | string | 否（可选配置） | 备注 |
| PCDCode | string | 否（可选配置） | 产地PCD代码 |
| PCDDescription | string | 否（可选配置） | 产地PCD描述 |
| GoodsWeight | decimal\(18,2\) | 否（可选配置） | 重量 |
| GoodsVolumn | decimal\(18,2\) | 否（可选配置） | 体积 |
| UnitSysNoList | array int | 否（可选配置） | 计量单位系统编码列表 |
| SpecGroup | object | 否 | 规格组（说明见”获取规格模板列表“） |
| AddSkuList | array object | 否 | 新增规格列表（说明见”新增款规格“） |
| PriceRuleType | int | 否（可选配置） | 定价规则：0按款定价，1按规格定价 |
| TagSysNoList | array int | 否（可选配置） | 标签列表 |
| BrandSysNoList | array int | 否（可选配置） | 品牌列表 |
| SupplierSysNoList | array int | 否（可选配置） | 供应商列表 |
| ProductServiceType | int | 否（可选配置） | 服务方式：0物流配送，1到店消费 |
| IsDisableRMA | int | 否（可选配置） | 是否禁用退货：0否，1是 |
| CommissionRate | decimal（18，4） | 否（可选配置） | 佣金比例 |
| EffectiveType | int | 否（可选配置） | 有效类型：0天数，1日期 |
| EffectiveDays | int | 否（可选配置） | 有效天数 |
| EffectiveDate | string | 否（可选配置） | 有效期 |
| EffectiveType | int | 否（可选配置） | 有效类型：0天数，1日期 |
| IsSupportPointPay | int | 否 | 是否支持积分支付 |
| RewardPoint | int | 否 | 奖励积分 |
| ServiceType | int | 否 | 消费方式（0按次数，1按时间） |
| ServiceOutMinutes | int | 否 | 过期时间（分钟）（0为长期有效） |
| GroupSysNos | Array\[int\] | 否 | 商品分组 |
| RewardMP | decimal | 否 | 奖励魔力 |
| FakeSaleCount | int | 否 | 虚假销量 |
| CPSMaterialUrl | string | 否 | CPS落地页 |
| CPSSysNo | int | 否 | CPS编码 |
| SourceCPSSysNo | int | 是 | 来源三方CPS |
| CPSStartDate | string | 否 | 三方CPS开始推荐 |
| CPSEndDate | string | 否 | 三方CPS结束推荐 |
| CPSInOrderCount | int | 否 | 三方CPS评价 |
| SourceProductGroupCode | string | 是 | 来源三方编码 |
| TaoWord | string | 是 | 淘口令 |
| FakeInventoryCount | int | 否 | 可砍份数 |
| StartSaleDate | datetime | 是 | 开卖时间 |
| GroupByCode | string | 否 | 多款聚合规格名称 |
| IsGroupByDefault | int | 否 | 多款聚合默认显示 |
| GroupByOtherName | string | 否 | 多款聚合别名 |
| ShopShowSourceList | array\[int\] | 否 | 展示来源（0普通，1蓝晶兑换） |
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
| Properties| int | 否 | 商品属性(Json字符串） |


#### _应答数据 _ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo | int | 是 | 系统编码 |




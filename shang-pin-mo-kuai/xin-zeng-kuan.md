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

#### _应答数据 _ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo | int | 是 | 系统编码 |




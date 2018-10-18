# 新增款规格 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增款规格

_**【应用场景】**_

新增款规格

注：只能修改属于自己数据范围结点内且IsCreator=1的商品；

注：SkuCode为空时的自动生产规则：款号+至少2位长度的该商品规格数量；

_**【接口地址】**_

[http://ip:port/ProductAction/](http://ip:port/HMAction/River/AddRiver)[S](http://ip:port/HMAction/River/AddRiver)ku[/A](http://ip:port/HMAction/River/AddRiver)ddProductSku

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ~~DataRangeSysNoList~~ | ~~array int~~ | ~~否~~ | ~~数据范围枝叶编码列表（必须在不同的树中的枝叶）~~ |
| ProductGroupSysNo | int | 是 | 款号系统编码 |
| AddSkuList | array object | 是 | 款规格列表 |

#### AddSku {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SkuName | string | 是 | sku名称 |
| SkuCode | string | 否（可选配置） | sku代码 |
| SkuDetail | string | 否（可选配置） | 详情 |
| SkuMemo | string | 否（可选配置） | 备注 |
| BarCode | string | 否（可选配置） | 条形码 |
| InternationalCode | string | 否（可选配置） | 国际码 |
| GoodsWeight | decimal\(18,2\) | 否（可选配置） | 重量 |
| GoodsVolumn | decimal\(18,2\) | 否（可选配置） | 体积 |
| AddSpecValueList | array object | 否（可选配置） | 规格值列表 |
| IsClearStocks | int | 否 | 是否限制库存：0否，1是 |
| FileMasterPathList | array string | 否（可选配置） | 主图图片列表 |
| ProductPrice | decimal\(18,2\) | 否（可选配置） | 价格（按规格定价时有效） |
| Quantity | int | 否 | 库存数量 |

> #### AddSpecValue {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SpecSysNo | int | 是 | 规格系统编码 |
| SpecValueSysNo | int | 是 | 规格值系统编码 |
| SpecValueOtherName | string | 否 | 规格值别名 |

> #### 应答_数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SkuSysNoList | array int| 是 | SKU系统编码 |






# 新增款规格 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增款规格

_**【应用场景】**_

新增款规格

注：“SkuName"与”SpecValueList“二选一必传；

注：只能修改属于自己数据范围结点内且IsCreator=1的商品；

_**【接口地址】**_

[http://ip:port/ProductAction/](http://ip:port/HMAction/River/AddRiver)[S](http://ip:port/HMAction/River/AddRiver)ku[/A](http://ip:port/HMAction/River/AddRiver)ddProductSku

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | array int | 是 | 数据范围枝叶编码列表（必须在不同的树中的枝叶） |
| ProductGroupSysNo | int | 是 | 款号系统编码 |
| AddSkuList | array object | 是 | 款规格列表 |

#### AddSku {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SkuName | string | 否 | sku名称 |
| SkuCode | string | 否 | sku代码 |
| SkuDetail | string | 否 | 详情 |
| SkuMemo | string | 否 | 备注 |
| BarCode | string | 否 | 条形码 |
| InternationalCode | string | 否 | 国际码 |
| GoodsWeight | decimal\(18,2\) | 否 | 重量 |
| GoodsVolumn | decimal\(18,2\) | 否 | 体积 |
| SpecValueList | array object | 否 | 规格值列表 |
| IsClearStocks | int | 否 | 是否限制库存：0否，1是 |

> #### SpecValue {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SpecValueSysNo | int | 是 | 规格值系统编码 |
| SpecOtherName | string | 否 | 规格值别名 |

> #### 应答_数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SkuSysNo | int | 是 | SKU系统编码 |




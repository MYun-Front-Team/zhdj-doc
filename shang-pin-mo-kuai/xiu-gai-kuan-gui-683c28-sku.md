# 新增款规格 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增款规格

_**【应用场景】**_

新增款规格

注：只能修改属于自己数据范围结点内且IsCreator=1的商品；

_**【接口地址】**_

[http://ip:port/ProductAction/](http://ip:port/HMAction/River/AddRiver)[S](http://ip:port/HMAction/River/AddRiver)ku[/E](http://ip:port/HMAction/River/AddRiver)ditProductSku

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ~~DataRangeSysNoList~~ | ~~array int~~ | ~~是~~ | ~~数据范围枝叶编码列表（必须在不同的树中的枝叶）~~ |
| ProductGroupSysNo | int | 是 | 款号系统编码 |
| EditSkuList | array object | 是 | 款规格列表 |

#### EditSku {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SkuSysNo | int | 是 | sku系统编码 |
| SkuName | string | 否 | sku名称 |
| SkuDetail | string | 否 | 详情 |
| SkuMemo | string | 否 | 备注 |
| BarCode | string | 否 | 条形码 |
| InternationalCode | string | 否 | 国际码 |
| GoodsWeight | decimal\(18,2\) | 否 | 重量 |
| GoodsVolumn | decimal\(18,2\) | 否 | 体积 |
| IsClearStocks | int | 否 | 是否限制库存：0否，1是 |
| AddSpecValueList | array object | 否 | 规格值列表（说明见新增） |
| FileMasterPathList | array string | 否 | 主图图片列表 |
| ProductPrice | decimal\(18,2\) | 否 | 价格（按规格定价时有效） |
| Quantity | int | 否 | 库存数量 |


> #### 应答_数据_ {#请求数据}




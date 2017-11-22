# 设置商品上下架状态 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

设置商品上下架状态

_**【应用场景】**_

设置商品上下架状态

注：只能修改属于自己数据范围结点内且IsCreator=1的商品；

注：该接口兼容款和sku的上下架功能，款的状态只能是1上架 2下架 4停售，而sku的状态只能是1上架 2下架，一旦操作的是sku的状态，则一般都会影响款的状态；

_**【接口地址】**_

[http://ip:port/ProductAction/](http://ip:port/HMAction/River/AddRiver)ProductGroup[/S](http://ip:port/HMAction/River/AddRiver)etProductOnSaleStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | array int | 是 | 数据范围枝叶编码列表（必须在不同的树中的枝叶） |
| ProductGroupSysNo | int | 是 | 款号系统编码 |
| SkuSysNoList | array int | 否 | 款规格列表 |
| OnSaleStatus | int | 是 | 上下状态:0待上架 1上架 2下架 3部分上架 4停售 |

> #### 应答_数据_ {#请求数据}




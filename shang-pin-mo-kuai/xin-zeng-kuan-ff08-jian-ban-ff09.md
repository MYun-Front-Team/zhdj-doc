# 新增款（简版） {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增款

_**【应用场景】**_

新增款，没有默认的规格模板的组织使用；

注：调用该接口说明该商品属于该组织，IsCreator=1；

注：ProductGroupCode为空时的自动生产规则：数据范围结点+至少3位长度的商品数量；

_**【接口地址】**_

[http://ip:port/ProductAction/](http://ip:port/HMAction/River/AddRiver)[P](http://ip:port/HMAction/River/AddRiver)roductGroup[/Add](http://ip:port/HMAction/River/AddRiver)ProductGroup2

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AddProductGroup | object | 是 | 新增款实体（见“新增款”） |
| SetProductImgList | object | 否 | 新增款图片（见“设置商品图片”） |
| ProductPrice | decimal\(18,2\) | 否 | 价格 |
| OnSaleStatus | int | 否 | 上下状态:0待上架 1上架 2下架 3部分上架 4停售 |
|IsHidden|int | 否 | 是否隐藏 |

#### _应答数据 _ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo | int | 是 | 系统编码 |




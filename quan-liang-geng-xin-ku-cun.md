# 全量更新库存 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

全量更新库存

_**【应用场景】**_

全量更新库存

注：全量更新库存定义：覆盖现有库存数量；

注：记录出库或入库日志到仓库模块中；

_**【接口地址】**_

[http://ip:port/WareHouseAction/](http://ip:port/HMAction/River/AddRiver)WareHouse[/E](http://ip:port/HMAction/River/AddRiver)ditInventoryQuantity

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionSysno | int | 是 | 库位系统编码 |
| SkuSysNo | int | 是 | 款规格系统编码 |
| Quantity | int | 是 | 更新数量 |
| BatchSysNo | int | 否 | 批次系统编码 |

> #### 应答_数据_ {#请求数据}




# 出库 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

出库

_**【应用场景】**_

出库

注：纪录出库日志到仓库模块中；

_**【接口地址】**_

[http://ip:port/WareHouseAction/](http://ip:port/HMAction/River/AddRiver)WareHouse[/S](http://ip:port/HMAction/River/AddRiver)etInventoryOut

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PositionSysno | int | 是 | 库位系统编码 |
| SkuSysNo | int | 是 | 款规格系统编码 |
| Quantity | int | 是 | 出库数量 |
| ReduceType | int | 是 | 类型：1盘亏，2其他出库， 3出库单出库 |
| VoucherNo | string | 否 | 出库单号 |
| BatchSysNo | int | 否 | 批次系统编码 |

> #### 应答_数据_ {#请求数据}




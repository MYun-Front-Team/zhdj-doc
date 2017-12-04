# 仓储模块-字段说明 {#新增河流}

> #### 商品款库存基础字段（ProductInventory） {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo | int | 是 | 款系统编码 |
| PhysicalQuantity | int | 是 | 物理库存 |
| AvailableQuantity | int | 是 | 可用库存 |
| VirtualQuantity | int | 是 | 虚拟库存 |
| FrozenQuantity | int | 是 | 冻结库存（含冻结库位库存+不可用库位库存+次品） |
| OrderLockQuantity | int | 是 | 订单锁数量 |
| DeliveryVoucherLockQuantity | int | 是 | 发货单锁数量 |
| SkuInventoryList | array object | 否 | 商品规格\(SKU\)库存列表 |

#### 注：可用库存=物理库存-冻结库存-订单锁数量-发货单锁数量+虚拟库存 {#请求数据}

#### 商品SKU库存基础字段（SkuInventory） {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SkuSysNo | int | 是 | 商品规格\(SKU\)系统编码 |
| PhysicalQuantity | int | 是 | 物理库存 |
| AvailableQuantity | int | 是 | 可用库存 |
| VirtualQuantity | int | 是 | 虚拟库存 |
| FrozenQuantity | int | 是 | 冻结库存（含冻结库位库存+不可用库位库存+次品） |
| OrderLockQuantity | int | 是 | 订单锁数量 |
| DeliveryVoucherLockQuantity | int | 是 | 发货单锁数量 |

#### 订单商品SKU锁库基础字段（OrderItemLockInventory） {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrderLockQuantity | int | 是 | 订单锁数量 |
| DeliveryVoucherLockQuantity | int | 是 | 发货单锁数量 |




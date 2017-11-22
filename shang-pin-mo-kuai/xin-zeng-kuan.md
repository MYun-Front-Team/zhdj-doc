# 新增款 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增款

_**【应用场景】**_

新增款

注：调用该接口说明该商品属于自己，IsCreator=1，新增商品到商品表并把商品与数据范围结点形成所属关系；

_**【接口地址】**_

[http://ip:port/ProductAction/](http://ip:port/HMAction/River/AddRiver)[P](http://ip:port/HMAction/River/AddRiver)roductGroup[/Add](http://ip:port/HMAction/River/AddRiver)ProductGroup

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | array int | 是 | 数据范围枝叶编码列表（必须在不同的树中的枝叶） |
| ProductType | int | 是 | 类型（枚举） |
| ProductClassSysNo | int | 否（可选配置） | 类型分类系统编码（类别树） |
| ProductGroupCode | string | 是 | 款号 |
| ProductGroupName | string | 是 | 款名称 |
| ProductGroupDetail | string | 否（可选配置） | 详情 |
| ProductGroupMemo | string | 否（可选配置） | 备注 |
| PCDCode | string | 否（可选配置） | 产地PCD代码 |
| PCDDescription | string | 否（可选配置） | 产地PCD描述 |
| GoodsWeight | decimal\(18,2\) | 否（可选配置） | 重量 |
| GoodsVolumn | decimal\(18,2\) | 否（可选配置） | 体积 |
| UnitSysNoList | array int | 否（可选配置） | 计量单位系统编码列表 |

#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo | int | 是 | 系统编码 |




# 删除款规格 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

删除款规格

_**【应用场景】**_

删除款规格

注：目前不需要判断业务数据中是否存在该商品规格；

_**【接口地址】**_

[http://ip:port/ProductAction/](http://ip:port/HMAction/River/AddRiver)[S](http://ip:port/HMAction/River/AddRiver)ku[/](http://ip:port/HMAction/River/AddRiver)DeleteProductSku

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ~~DataRangeSysNoList~~ | ~~array int~~ | ~~是~~ | ~~数据范围枝叶编码列表（必须在不同的树中的枝叶）~~ |
| ProductGroupSysNo | int | 是 | 款号系统编码 |
| SkuSysNoList | array int | 是 | 款规格系统编码列表 |

> #### 应答_数据_ {#请求数据}




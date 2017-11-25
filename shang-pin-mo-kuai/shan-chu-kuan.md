# 删除款 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

删除款

_**【应用场景】**_

删除款

注：判断商品与数据范围是否存在引入，无则只删除组织与商品的关系，有则提示不允许删除；

_**【接口地址】**_

[http://ip:port/ProductAction/](http://ip:port/HMAction/River/AddRiver)[P](http://ip:port/HMAction/River/AddRiver)roductGroup[/D](http://ip:port/HMAction/River/AddRiver)eleteProductGroup

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ~~DataRangeSysNoList~~ | ~~array int~~ | ~~是~~ | ~~数据范围枝叶编码列表（必须在不同的树中的枝叶）~~ |
| ProductGroupSysNoList | array int | 是 | 款号系统编码列表 |

#### _应答数据_ {#应答数据-}




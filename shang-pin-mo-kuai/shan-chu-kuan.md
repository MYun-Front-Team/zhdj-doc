# 删除款 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

删除款

_**【应用场景】**_

删除款

注：通用UserSysNo找到所属全部数据范围结点，并与参数DataRangeSysNoList进行判断；

注：只能删除属于自己数据范围结点内的商品；

_**【接口地址】**_

[http://ip:port/ProductAction/](http://ip:port/HMAction/River/AddRiver)[P](http://ip:port/HMAction/River/AddRiver)roductGroup[/D](http://ip:port/HMAction/River/AddRiver)eleteProductGroup

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | array int | 是 | 数据范围枝叶编码列表（必须在不同的树中的枝叶） |
| ProductGroupSysNoList | array int | 是 | 款号系统编码列表 |

#### _应答数据_ {#应答数据-}




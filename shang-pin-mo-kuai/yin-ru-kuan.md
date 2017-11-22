# 引入款 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

引入款

_**【应用场景】**_

引入款

注：通用UserSysNo找到所属全部数据范围结点，并与参数DataRangeSysNoList进行判断；

注：引入款的IsCreator=0，后续不允许修改；

_**【接口地址】**_

[http://ip:port/ProductAction/](http://ip:port/HMAction/River/AddRiver)[P](http://ip:port/HMAction/River/AddRiver)roductGroup[/P](http://ip:port/HMAction/River/AddRiver)ullProductGroup

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | array int | 是 | 数据范围枝叶编码列表（必须在不同的树中的枝叶） |
| PullProductGroupList | array object | 是 | 引入款列表 |

#### PullProductGroup {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupSysNo | int | 是 | 款号系统编码 |
| SkuSysNoList | array int | 是 | SKU系统编码列表 |

> #### 应答_数据_ {#请求数据}




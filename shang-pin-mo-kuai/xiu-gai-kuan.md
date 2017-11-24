# 修改款 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改款

_**【应用场景】**_

修改款

注：通用UserSysNo找到所属全部数据范围结点，并与参数DataRangeSysNoList进行判断；

注：只能修改属于自己数据范围结点内且IsCreator=1的商品；

_**【接口地址】**_

[http://ip:port/ProductAction/](http://ip:port/HMAction/River/AddRiver)[P](http://ip:port/HMAction/River/AddRiver)roductGroup[/E](http://ip:port/HMAction/River/AddRiver)ditProductGroup

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | array int | 是 | 数据范围枝叶编码列表（必须在不同的树中的枝叶） |
| ProductGroupSysNo | int | 是 | 款号系统编码 |
| ProductClassSysNo | int | 否（可选配置） | 类型分类系统编码（类别树） |
| ProductGroupName | string | 是 | 款名称 |
| ProductGroupDetail | string | 否（可选配置） | 详情 |
| ProductGroupMemo | string | 否（可选配置） | 备注 |
| PCDCode | string | 否（可选配置） | 产地PCD代码 |
| PCDDescription | string | 否（可选配置） | 产地PCD描述 |
| GoodsWeight | decimal\(18,2\) | 否（可选配置） | 重量 |
| GoodsVolumn | decimal\(18,2\) | 否（可选配置） | 体积 |
| UnitSysNoList | array int | 否（可选配置） | 计量单位系统编码列表 |
| SpecGroup | object | 否 | 规格组（说明见”获取规格模板列表“） |
| EditSkuList | array object | 否 | 修改规格列表（说明见”新增款规格“） |

#### _应答数据_ {#应答数据-}




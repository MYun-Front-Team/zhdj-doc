# 删除规格模板 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

删除规格模板

_**【应用场景】**_

删除规格模板

注：当SpecValueSysNoList为空时，删除规格，否则删除规格值；

_**【接口地址】**_

[http://ip:port/ProductAction/Spec/D](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)eleteSpecTemplate

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SpecSysNo | int | 是 | 商品规格系统编码 |
| SpecValueSysNoList | array int | 否 | 商品规格值系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




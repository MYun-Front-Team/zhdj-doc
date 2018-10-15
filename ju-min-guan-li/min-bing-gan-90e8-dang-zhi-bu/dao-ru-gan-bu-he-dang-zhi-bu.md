# 导入干部和党支部

##### _【功能说明】_ {#【功能说明】}
导入干部和党支部

_**【应用场景】**_

导入干部和党支部

_**【接口地址】**_

http://ip:port/ResidentAction/Resident/ImportResidentSoldier

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ResidentSoldiers| array[ResidentSoldierAdd] | 是 | 民兵 |
| SoldierType| int | 是 | 民兵类型（1干部2党支部） |


 #### ResidentSoldierAdd

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeName| string | 是 | 数据范围树名称 |
| Sex| int | 是 | 性别：1男，2女 |
| Name| string | 是 | 姓名 |
| CellPhoneNo| string  | 是 | 手机号|
| Post| int | 是 | 党内职务：10书记，20副书记，30组织委员，40宣传委员,50纪检委员，60工青妇委员,70组织员 ; 干部职务：100营长，110营政治辅导员,120副营长，130营副政治辅导员，200连长，210连政治辅导员220副连长，230连副政治辅导员， |
| CellPhoneNo| string  | 是 | 手机号|












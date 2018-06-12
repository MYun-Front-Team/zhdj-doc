#新增业主

##### _【功能说明】_ {#【功能说明】}

新增业主

_**【应用场景】**_

新增业主

_**【接口地址】**_
http://ip:port/ResidentAction/Resident/AddResidentOwners



> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ResidentOwners| array[ResidentOwner] | 是 |业主|


 #### ResidentOwner

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 数据范围树枝叶编码 |
| RoomNo | string | 是 | 房间编号 |
| CellPhoneNo| string | 是 | 手机号 |
| PersonName| string | 是 | 业主名称 |
| Area| decimal| 是 | 面积 |
| IDCard| string | 否 | 身份证号 |
| Remark| string | 否 |备注|






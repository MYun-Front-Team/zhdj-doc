#获取业主详情

##### _【功能说明】_ {#【功能说明】}

获取业主详情

_**【应用场景】**_
获取业主详情

_**【接口地址】**_

http://ip:port/ResidentQuery/Resident/GetResidentOwnerBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ResidentOwnerSysNo | int | 是 | 系统编码 |



> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ResidentOwnerSysNo | int | 是 | 系统编码 |
| DataRangeSysNo | int | 是 | 数据范围树枝叶编码 |
| DataRangeName | string| 是 | 数据范围树枝叶名称 |
| RoomNo | string | 否 | 房间编号 |
| CellPhoneNo| string | 否 | 手机号 |
| PersonName| string | 否 | 业主名称 |
| Area| decimal| 否 | 面积 |
| IDCard| string | 否 | 身份证号 |
| Remark| string | 否 |备注|


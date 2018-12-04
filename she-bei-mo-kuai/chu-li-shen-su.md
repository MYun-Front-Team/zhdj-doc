# 处理申诉 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/EqmAction/Equipment/DealComplain](http://ip:port/EqmQuery/Equipment/GetEquipmentBySysNo)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ComplainSysNo | int | 是 | 申诉编码 |
| PersonSysNo | int | 是 | 处理人员编码 |
| DealStatus | int | 是 | 10同意，11拒绝 |
| RefuseReason | string | 否 | 拒绝理由 |
|  |  |  |  |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |





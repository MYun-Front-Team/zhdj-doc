# 提交申诉单 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/EqmAction/Equipment/AddComplain](http://ip:port/EqmQuery/Equipment/GetEquipmentBySysNo)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 申诉人员编码 |
| OrderSysNo | int | 是 | 订单编码 |
| Reason | string | 否 | 申诉理由 |
| ContactPhone | string | 是 | 联系电话 |
| FileUrlList | array string | 否 | 凭证列表 |
|  |  |  |  |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 申诉编码 |




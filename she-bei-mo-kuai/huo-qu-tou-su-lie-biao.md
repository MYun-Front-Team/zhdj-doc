# 获取投诉列表 {#获取河长巡河记录}

_**【接口地址】**_

http://ip:port/EqmQuery/Equipment/GetComplainList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 否 | 运营商人员编码 |
| CustomerPersonSysNo | int | 否 | 消费者人员编码 |
| ComplainStatusList | array\[int\] | 否 | 1未处理，10已处理 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 总数 |
| PersonName | string | 是 | 昵称 |
| AvatarUrl | string | 是 | 头像 |
| ContactPhone | string | 是 | 联系方式 |




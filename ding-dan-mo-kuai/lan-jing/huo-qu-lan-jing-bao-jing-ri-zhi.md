# 获取蓝晶报警日志

获取蓝晶报警日志

_**【应用场景】**_

获取蓝晶报警日志

_**【接口地址】**_

http://ip:port/PointsQuery/LJPoint/GetLJPointWarningLog

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| KeyWord| string| 否 |转出人关键字 |
| PersonSysNo| int | 否 |转出人员系统编码 |
| StartCreateTime| datetime| 否 |开始创建|
| EndCreateTime| datetime| 否 |终止创建|


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WarningLogSysNo| int| 是 |系统编码|
| PersonName| string| 是 | 转出人|
| CellPhoneNo| string| 是 |转出人手机|
| ChangePointsValue| decimal | 否 | 过去7天转出蓝晶（负数）|
| CreateTime| datetime| 否 |报警时间|




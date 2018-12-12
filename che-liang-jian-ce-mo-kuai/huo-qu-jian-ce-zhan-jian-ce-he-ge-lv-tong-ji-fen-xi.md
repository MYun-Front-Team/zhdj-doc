# 获取检测站检测合格率统计分析 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/VDQuery/Detect/GetDSDetectPassPercent](http://ip:port/EqmQuery/Equipment/GetEquipmentList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| dsName | string | 否 | 检测机构名称 |
| StartDate | datetime | 否 | 开始日期 |
| EndDate | datetime | 否 | 结束日期 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OncePassPercent | decimal | 是 | 一次合格率 |
| SecondaryPassPercent | decimal | 是 | 二次合格率 |
| OtherPassPercent | decimal | 是 | 其他 |




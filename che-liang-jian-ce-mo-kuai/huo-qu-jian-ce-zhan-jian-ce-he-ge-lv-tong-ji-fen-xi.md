# 获取检测站检测合格率统计分析 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/VDQuery/Detect/GetDSDetectPassPercent](http://ip:port/EqmQuery/Equipment/GetEquipmentList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| dsName | string | 否 | 检测机构名称 |
| StartDate | datetime | 否 | 开始日期 |
| EndDate | datetime | 否 | 结束日期 |
| AreaCode | string | 否 | 区域编号 |
| detectType | int | 否 | 1.动力性 2.经济性  3. 第一转向轮 4 第二转向轮 |


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OncePassPercent | decimal | 是 | 一次合格率 |
| SecondaryPassPercent | decimal | 是 | 二次合格率 |
| OtherPassPercent | decimal | 是 | 其他 |
| NoPassPercent | decimal | 是 | 不合格率 |



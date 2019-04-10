#获取委托人统计列表

_**【接口地址】**_

http://ip:port/VDQuery/Detect/GetClientDetectPassList

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StartDate | datetime | 否 | 开始日期 |
| EndDate | datetime | 否 | 结束日期 |

> #### _应答数据 _

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Client | string | 否 | 委托人 |
| PassPercent | decimal | 是 | 合格率 |
| NoPassPercent | decimal | 是 | 不合格率 |

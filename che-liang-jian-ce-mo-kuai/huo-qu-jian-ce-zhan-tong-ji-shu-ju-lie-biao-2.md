# 获取检测站统计数据列表2

_**【接口地址】**_

http://ip:port/VDQuery/Detect/GetDSDetectPassList2

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StartDate | datetime | 否 | 开始日期 |
| EndDate | datetime | 否 | 结束日期 |
| AreaCode | string | 否 | 区域编号 |



> #### _应答数据 _

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| dsId | string | 是 | 检测机构代码 |
| dsName | string | 是 | 检测机构名称 |
| OncePassPercent1 | decimal | 是 | 动力性一次合格率 |
| SecondaryPassPercent1 | decimal | 是 | 动力性二次合格率 |
| OtherPassPercent1 | decimal | 是 | 动力性其他 |
| NoPassPercent1 | decimal | 是 | 动力性不合格率 |
| OncePassPercent2 | decimal | 是 | 经济性一次合格率 |
| SecondaryPassPercent2 | decimal | 是 | 经济性二次合格率 |
| OtherPassPercent2 | decimal | 是 | 经济性其他 |
| NoPassPercent2 | decimal | 是 | 经济性不合格率 |
| OncePassPercent3 | decimal | 是 | 第一转向轮一次合格率 |
| SecondaryPassPercent3 | decimal | 是 | 第一转向轮二次合格率 |
| OtherPassPercent3 | decimal | 是 | 第一转向轮其他 |
| NoPassPercent3 | decimal | 是 | 第一转向轮不合格率 |
| OncePassPercent4 | decimal | 是 | 第二转向轮一次合格率 |
| SecondaryPassPercent4 | decimal | 是 | 第二转向轮二次合格率 |
| OtherPassPercent4 | decimal | 是 | 第二转向轮其他 |
| NoPassPercent4 | decimal | 是 | 第二转向轮不合格率 |

#获取检测站统计列表

_**【接口地址】**_

http://ip:port/VDQuery/Detect/GetDSDetectPassList

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
| detectType | int | 是 | 1.动力性 2.经济性  3. 第一转向轮 4 第二转向轮 |
| OncePassPercent | decimal | 是 | 一次合格率 |
| SecondaryPassPercent | decimal | 是 | 二次合格率 |
| OtherPassPercent | decimal | 是 | 其他 |
| NoPassPercent | decimal | 是 | 不合格率 |

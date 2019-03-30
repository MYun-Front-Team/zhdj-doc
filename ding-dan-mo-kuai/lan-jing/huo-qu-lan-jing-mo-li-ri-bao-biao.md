# 获取蓝晶魔力日报表

获取蓝晶魔力日报表

_**【应用场景】**_

获取蓝晶魔力日报表
_**【接口地址】**_

http://ip:port/PointsQuery/LJPoint/GetLJPointReport




#### 查询条件字段 {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StartReportDate| datetime | 否 |开始日报时间 |
| EndReportDate| datetime | 否 |结束日报时间 |


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

#### Group {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ReportDate| datetime| 是 | 报表时间|
| DayFrozenMP| decimal| 是 | 当日冻结魔力|
| TaskMP| decimal| 是 | 任务空投魔力|
| SettlementMP| decimal| 是 | 当日结算魔力|
| GiveMP| decimal| 是 | 平台空投魔力|
| AllFrozenMP| decimal| 是 | 累计冻结魔力|
| TransforLJ| decimal| 是 | 蓝晶合成|
| GiveLJ| decimal| 是 | 蓝晶转赠|
| GiveLJCount| decimal| 是 |蓝晶转增比数|
| LJToOrderCount| decimal| 是 | 蓝晶兑换比数|
| LJToOrder| decimal| 是 | 蓝晶兑换|

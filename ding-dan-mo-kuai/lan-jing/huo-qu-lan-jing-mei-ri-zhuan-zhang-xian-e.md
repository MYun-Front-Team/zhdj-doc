# 获取蓝晶每日转账限额

获取蓝晶每日转账限额

_**【应用场景】**_

获取蓝晶每日转账限额

_**【接口地址】**_

http://ip:port/PointsQuery/LJPoint/GetLJPointTransferLimit

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo| int | 否 |转出人员系统编码 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MaxPointsValue| decimal| 是 |每日蓝晶额度|
| OutChangePointsValue| decimal| 是 |每日已用额度|
| LeftPointsValue| decimal| 是 |剩余蓝晶额度|


# 获取蓝晶转赠记录日志

获取蓝晶转赠记录日志

_**【应用场景】**_

获取蓝晶转赠记录日志

_**【接口地址】**_

http://ip:port/PointsQuery/LJPoint/GetLJPointTransferLog

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| KeyWord| string| 否 |转出人关键字 |
| OutPersonSysNo| int | 否 |转出人员系统编码 |
| StartCreateTime| datetime| 否 |开始创建|
| EndCreateTime| datetime| 否 |终止创建|
| StartChangePointsValue| decimal| 是 |起始蓝晶（正数）|
| EndChangePointsValue| decimal| 是 |终止蓝晶（正数）|

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ChangePointsValue| decimal| 是 |蓝晶（负数）|
| Remark| string| 是 | 备注|
| CreateTime| datetime| 是 |创建时间|
| FileUrlList | array string | 否 | 头像图片列表（仅转账操作才有值） |
| OutPersonName| string | 否 | 转出人员昵称（仅转账操作才有值） |
| OutCellPhoneNo| string | 否 | 转出人员手机（仅转账操作才有值） |
| InPersonName| string | 否 | 接收人员昵称（仅转账操作才有值） |
| InCellPhoneNo| string | 否 | 接收人员手机（仅转账操作才有值） |

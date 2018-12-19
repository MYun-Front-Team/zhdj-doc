# 魔力/蓝晶转账

魔力/蓝晶转账

_**【应用场景】**_

魔力/蓝晶转账

_**【接口地址】**_

http://ip:port/PointsAction/LJPoint/TransferLJPoint

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PointsType| int | 是 |积分类型（1蓝晶/2魔力） |
| FromPersonSysNo| int | 是 |转出人员系统编码 |
| ToPersonSysNo| int | 是 |转入人员系统编码 |
| PointsValue| decimal| 是 | 魔力/蓝晶数量|
| Captcha | string | 否 | 验证码（短信登录时必填） |
| CellPhoneNo| string | 否| 手机号 | 




> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |







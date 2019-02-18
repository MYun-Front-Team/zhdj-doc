# 获取微信好友

_**【接口地址】**_

http://ip:port/MessageQuery/Message/GetWechatFriendList

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 否 | 人员编码 |
| Keywords | string | 否 | 关键字 |
| DeviceSysNoList | array int | 否 | 设备id列表 |

> #### _应答数据 _

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SysNo | int | 是 | 系统编码 |
| PersonSysNo | int | 是 | 人员编码 |
| DeviceStatusSysNo | int | 是 | 设备id |
| DeviceName | string | 是 | 设备名称 |
| DeviceCode | string | 是 | 设备编号 |
| WechatNo | string | 是 | 好友id |
| NickName | string | 是 | 好友名称 |



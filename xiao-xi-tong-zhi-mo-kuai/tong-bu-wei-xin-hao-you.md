# 同步微信好友

_**【接口地址】**_

http://ip:port/MessageAction/Message/SyncWechatFriends

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员编码 |
| DeviceSysNo | int | 是 | 设备id |
| DataList | array[object] | 是 | 好友列表 |

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| id | string | 是 | 好友id |
| name | string | 是 | 好友名称 |


> #### _应答数据 _

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |





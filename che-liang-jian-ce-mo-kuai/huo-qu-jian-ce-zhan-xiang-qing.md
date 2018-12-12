# 获取检测站详情 {#获取河长巡河记录}

_**【接口地址】**_

http://ip:port/VDQuery/Detect/GetDSBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| dsSysNo | int | 是 | 检测站id |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| dsSysNo | int | 是 | 检测站id |
| LoginId | string | 是 | 登录账号 |
| Password | string | 是 | 登录密码 |
| dsName | string | 是 | 检测机构名称 |
| dsAddress | string | 是 | 检测机构地址 |
| dsTel | string | 是 | 服务热线 |
| uploadTime | int | 是 | 上传时间，秒数 |
| uploadCount | int | 是 | 每次上传检测数 |




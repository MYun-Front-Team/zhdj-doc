# 获取检测站列表 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/VDQuery/Detect/GetDSList](http://ip:port/VDQuery/Detect/GetDSList)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AreaCode | string | 否 | 区域编号 |
| CMALeftDay | int | 否 | 1，未知，2未过期，3已过期 |
| Keywords | string | 否 | 关键字 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| dsSysNo | int | 是 | 检测站id |
| AdminSysNo | int | 是 | 用户id |
| dsId | string | 是 | 检测机构代码 |
| LoginId | string | 是 | 登录账号 |
| Password | string | 是 | 登录密码 |
| dsName | string | 是 | 检测机构名称 |
| dsAddress | string | 是 | 检测机构地址 |
| dsTel | string | 是 | 服务热线 |
| uploadTime | int | 是 | 上传时间，秒数 |
| uploadCount | int | 是 | 每次上传检测数 |
| IsEnable | int | 是 | 1启用，2禁用 |
| detectRecorduploadCount | int | 是 | 上传报告数 |
| detectRecordSuccessCount | int | 是 | 成功报告数 |
| CMAUrl | string | 是 | CMA证书url |
| CMAStartDate | datetime | 是 | CMA证书有效期始 |
| CMAEndDate | datetime | 是 | CMA证书有效期止 |
| CMALeftDay | int | 是 | CMA证书剩余有效期 |
| VideoUrl | string | 是 | 视频url |
| AreaCode | string | 是 | 区域编号 |
| AreaName | string | 是 | 区域名称 |
| DeviceNum | int | 是 | 设备数量 |

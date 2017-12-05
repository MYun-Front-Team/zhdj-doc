# 修改工单 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改工单

_**【应用场景】**_

修改工单

_**【接口地址】**_

[http://ip:port/WorkAction/](http://ip:port/HMAction/River/AddRiver)Work/EditWork

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WorkSysNo | int | 是 | 系统编码 |
| WorkTitle | string | 否 | 标题 |
| WorkContent | string | 否 | 内容 |
| WorkTime | string | 否 | 发生时间 |
| PCDCode | string | 否 | 省市区 代码 |
| PCDDescription | string | 否 | 省市区 名称 |
| WorkAddress | string | 否 | 发生地地址 |
| Longitude | decimal（18，10） | 否 | 经度 |
| Latitude | decimal（18，10） | 否 | 纬度 |
| Remark | string | 否 | 备注 |
| FilePathList | array string | 否 | 文件或图片Path列表（第一张为首图） |

#### _应答数据_ {#应答数据-}




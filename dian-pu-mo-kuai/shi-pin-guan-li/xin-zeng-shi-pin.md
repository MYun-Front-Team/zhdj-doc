# 新增视频 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增视频

_**【应用场景】**_

新增视频

注（端）：视频的存储在阿里云的视频点播模块，可调用EDI来获取“VideoID”；

_**【接口地址】**_

[http://ip:port/ShopAction/Video/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddVideo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织系统编码 |
| VideoTitle | string | 是 | 视频标题 |
| VideoID | string | 否 | 第三方视频ID |
| VideoPathList | array string | 否 | 视频主图path路径 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| VideoSysNo | int | 是 | 视频系统编码 |




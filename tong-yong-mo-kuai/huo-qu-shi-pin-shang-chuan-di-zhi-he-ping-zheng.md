# 获取视频上传地址和凭证

##### _【功能说明】_ {#【功能说明】}

获取视频上传地址和凭证

_**【应用场景】**_

获取视频上传地址和凭证

_**【接口地址】**_

http://ip:port/UMAction/Video/UploadCreate

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Title | string | 是 | 视频标题，长度不超过128个字节，UTF8编码 |
| FileName| string | 是 | 视频源文件名，必须带扩展名，且扩展名不区分大小写 |
| FileSize| string | 否 | 视频文件大小，单位：字节 |
| Description| string | 否 |视频描述，长度不超过1024个字节，UTF8编码 |
| CoverURL| string | 否 |自定义视频封面URL地址 |
| CateId| long | 否 |视频分类ID，请在“点播控制台-全局设置-分类管理”里编辑或查看分类的ID|
| Tags| string | 否 |视频标签，单个标签不超过32字节，最多不超过16个标签。多个用逗号分隔，UTF8编码|

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RequestId | string | 是 | 请求ID。 |
| VideoId | string | 是 | 视频ID。|
| UploadAddress| string | 是 |上传地址。 |
| UploadAuth| string | 是 | 上传凭证。 |


























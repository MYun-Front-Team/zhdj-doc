# 获取视频播放地址

##### _【功能说明】_ {#【功能说明】}

获取视频播放地址

_**【应用场景】**_

获取视频播放地址

_**【接口地址】**_

http://ip:port/UMQuery/Video/GetVideoAuth

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| VideoId | string | 是 | 视频ID |
| Formats| string | 否 | 视频流格式，多个用逗号分隔，支持格式mp4,m3u8,mp3，默认获取所有格式的流 |
| AuthTimeout| string | 否 | 播放鉴权过期时间，默认为1800秒，支持设置最小值为1800秒 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| RequestId | string | 是 | 请求ID。 |
| VideoMeta | VideoMeta | 是 |视频meta信息|
| PlayAuth|string | 是 |视频播放凭证 |


### VideoMeta

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
|VideoId| 	String | 是 |	视频ID。|
|Title| 	String | 是 |	视频标题。|
|Duration| 	Float| 是 | 	视频时长(秒)。|
|CoverURL| 	String| 是 | 	视频封面。|
|Status| 	String | 是 |	视频状态。|


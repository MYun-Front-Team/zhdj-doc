# 获取视频播放地址

##### _【功能说明】_ {#【功能说明】}

获取视频播放地址

_**【应用场景】**_

获取视频播放地址

_**【接口地址】**_

http://ip:port/UMQuery/Video/GetVideo

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
| VideoBase | VideoBase | 是 | 视频基本信息|
| PlayInfoList| PlayInfo[]  | 是 |视频流信息列表 |


### VideoBase

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| VideoId| String|是 | 视频ID|
|Title|	String|是 |视频标题|
|Duration|String|是 | 视频时长(秒)|
|CoverURL |String|是 | 视频封面|
|Status|String|是 | 视频状态|
|CreationTime|String|是 | 视频创建时间，为UTC时间|
|MediaType|String|是 |媒体文件类型。取值范围 video(视频)audio(纯音频)|

### PlayInfo

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
|Bitrate|String|是 | 视频流码率，单位Kbps|
|Definition|String|是 | 视频流清晰度定义。取值范围：FD（流畅）LD（标清）SD（高清）HD（超清）OD（原画）2K（2K）4K（4K）| 
|Duration|String|是 | 视频流长度，单位秒|
|Encrypt|Long|是 | 视频流是否加密流。取值范围：0（否）1（是）| 
|PlayURL|String	|是 | 视频流的播放地址。|
|Format|String|是 | 视频流格式。若媒体文件为视频，取值范围：mp4 m3u8 若是纯音频，取值范围：mp3|
|Fps|String|是 | 视频流帧率，每秒多少帧。|
|Size|Long|是 | 视频流大小，单位Byte。|
|Width|Long|是 | 视频流宽度，单位px。|
|Height|Long|是 | 视频流高度，单位px|
|StreamType|String|是 | 视频流类型。若媒体流为视频，取值范围：video 若是纯音频，取值范围：audio|
|JobId|String|是 | 媒体流转码的作业ID，作为媒体流的唯一标识。|


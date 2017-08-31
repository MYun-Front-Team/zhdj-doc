# 新增回复 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增回复

_**【应用场景】**_

新增回复

_**【接口地址】**_

[http://ip:port/UMAction/Info/Add](http://ip:port/HMAction/River/AddRiver)InfoReply

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InfoSysNo | int | 否（与Source二选一必填） | 资讯系统编码 |
| SourceType | int | 否 | 类型：0客户，1用户 |
| SourceSysNo | int | 否 | 对应系统编码 |
| ReplyTime | string | 否 | 时间 |
| ReplyTitle | string | 否 | 主题 |
| ReplyContent | string | 否 | 内容 |
| ReplyJson | string | 否 | 端自定义字段（原样返回） |
| Remark | string | 否 | 备注 |
| FilePaths | string | 否 | 文件图片路径列表 |
| ~~SourceOperateType~~ | ~~int~~ | ~~否~~ | ~~来源操作类型：0新增，1查看，2回复，3审核，4上传，5下载，6签到，10完结（如传该参数，则判断是否需要赠送积分）~~ |

#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ReplySysNo | int | 是 | 回复系统编码 |




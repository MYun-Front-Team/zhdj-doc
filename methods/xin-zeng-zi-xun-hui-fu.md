# 新增资讯回复 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增资讯回复

_**【应用场景】**_

新增资讯回复

_**【接口地址】**_

[http://ip:port/UMAction/Info/Add](http://ip:port/HMAction/River/AddRiver)InfoReply

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InfoSysNo | int | 否（与Source二选一） | 资讯系统编码 |
| SourceType | int | 否 | 类型 |
| SourceSysNo | int | 否 | 对应系统编码 |
| ReplyTitle | string | 否 | 主题 |
| ReplyContent | string | 否 | 内容 |
| ReplyJson | string | 否 | 端自定义JSON |
| Remark | string | 否 | 备注 |

#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FootPrintSysNo | int | 是 | 足迹系统编码 |




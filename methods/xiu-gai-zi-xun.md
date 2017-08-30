# 修改资讯 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改资讯

_**【应用场景】**_

修改资讯

_**【接口地址】**_

[http://ip:port/UMAction/Info/E](http://ip:port/HMAction/River/AddRiver)ditInfo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InfoSysNo | int | 是 | 资讯系统编码 |
| InfoClassSysNo | int | 否 | 资讯分类系统编码 |
| InfoTitle | string | 否 | 资讯标题（主题） |
| InfoContent | string | 否 | 资讯内容 |
| MaxPersonNum | int | 否 | 人数上限 |
| InfoSignUpStartTime | string | 否 | 报名开始时间 |
| InfoSignUpEndTime | string | 否 | 报名结束时间 |
| InfoStartTime | string | 否 | 活动开始时间 |
| InfoEndTime | string | 否 | 活动结束时间 |
| InfoPlace | string | 否 | 活动地点 |
| RelationJson | string | 否 | 端自定义JSON（原样返回） |
| FilePaths | array string | 否 | 文件或图片列表（第一张为首图） |
| Auths | array object | 否 | 可见权限 |

####  {#应答数据-}




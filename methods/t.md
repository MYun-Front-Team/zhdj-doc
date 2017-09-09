# 新增活动 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增活动

_**【应用场景】**_

新增活动

_**【接口地址】**_

[http://ip:port/ActivityAction/Activity/Add](http://ip:port/HMAction/River/AddRiver)Activity

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SourceType | int | 是 | 归属类型：0客户，1用户，2部门 |
| SourceSysNo | int | 是 | 归属系统编码（支部编码） |
| InfoTypeSysNo | int | 是 | 资讯模块类型系统编码（见概述） |
| InfoClassSysNo | int | 否 | 资讯分类系统编码 |
| InfoTitle | string | 是 | 资讯标题（主题） |
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
| PointsConfigs | array object | 否 | 积分赠送配置 |
| Propertys | array object | 否 | 属性列表（见通用属性列表） |

#### PointsConfigs说明 {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SourceOperateType | int | 是 | 来源操作类型：0新增，1查看，2回复，3审核，4上传，5下载，6签到，10完结 |
| PointsValue | int | 是 | 积分值 |

#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InfoSysNo | int | 是 | 资讯系统编码 |




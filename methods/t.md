# 新增活动 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

活动模块-新增活动

_**【应用场景】**_

先获取新增活动页字段列表接口和积分配置列表接口，再新增活动。

_**【接口地址】**_

[http://ip:port/ActivityAction/Activity/Add](http://ip:port/HMAction/River/AddRiver)Activity

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ActivityType | int | 是 | 类型（枚举） |
| ActivityClassSysNo | int | 否 | 类型分类系统编码（类别树） |
| ActivityTitle | string | 是 | 标题 |
| ActivityContent | string | 否 | 内容 |
| MaxPersonNum | int | 否 | 人数上限 |
| ActivitySignUpStartTime | string | 否 | 报名开始时间 |
| ActivitySignUpEndTime | string | 否 | 报名结束时间 |
| ActivityStartTime | string | 否 | 活动开始时间 |
| ActivityEndTime | string | 否 | 活动结束时间 |
| ActivityPlace | string | 否 | 活动地点 |
| ActivitySummary | string | 否 | 活动记要 |
| FilePaths | array string | 否 | 文件或图片列表（第一张为首图） |
| PointsValues | array object | 否 | 积分赠送配置 |
| ~~Propertys~~ | ~~array object~~ | ~~否~~ | ~~属性列表（见通用属性列表）~~ |

#### PointsValues说明 {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PointsConfigSysNo | int | 是 | 积分配置系统编码 |
| PointsValue | int | 是 | 积分值 |

#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| InfoSysNo | int | 是 | 资讯系统编码 |




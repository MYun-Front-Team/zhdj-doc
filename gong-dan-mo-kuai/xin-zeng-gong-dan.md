# 新增工单 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增工单

_**【应用场景】**_

新增工单

_**【接口地址】**_

[http://ip:port/WorkAction/](http://ip:port/HMAction/River/AddRiver)Work/AddWork

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 工单所属数据范围系统编码 |
| ToPersonSysNo | int | 否（可选配置） | 处理人员系统编码 |
| WorkType | int | 是 | 类型（枚举） |
| WorkClassSysNo | int | 否（可选配置） | 类型分类系统编码（类别树） |
| WorkTitle | string | 否（可选配置） | 标题 |
| WorkContent | string | 是 | 内容 |
| WorkTime | string | 否（可选配置） | 发生时间 |
| PCDCode | string | 否 | 省市区 代码 |
| PCDDescription | string | 否 | 省市区 名称 |
| WorkAddress | string | 否 | 发生地地址 |
| Longitude | decimal（18，10） | 否 | 经度 |
| Latitude | decimal（18，10） | 否 | 纬度 |
| SponsorName | string | 否（可选配置） | 主办方 |
| CoSponsorName | string | 否（可选配置） | 协办方 |
| Remark | string | 否（可选配置） | 备注 |
| FilePathList | array string | 否（可选配置） | 文件或图片Path列表（第一张为首图） |
| TagSysNoList | array int | 否（可选配置） | 标签列表 |

#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WorkSysNo | int | 是 | 系统编码 |




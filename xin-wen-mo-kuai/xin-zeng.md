# 新增 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新闻模块-新增

_**【应用场景】**_

先根据页面，获取可选字段列表接口和积分配置列表接口，再新增。

_**【接口地址】**_

[http://ip:port/NewsAction/](http://ip:port/HMAction/River/AddRiver)[News](http://ip:port/HMAction/River/AddRiver)[/Add](http://ip:port/HMAction/River/AddRiver)[News](http://ip:port/HMAction/River/AddRiver)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | array int | 是 | 数据范围枝叶编码列表（必须在不同的树中的枝叶） |
| NewsType | int | 是 | 类型（枚举） |
| NewsClassSysNo | int | 否（可选配置） | 类型分类系统编码（类别树） |
| NewsTitle | string | 是 | 标题 |
| NewsContent | string | 是 | 内容 |
| Remark | string | 否（可选配置） | 备注 |
| IsNeedMoments | int | 否（可选配置） | 是否需要关联朋友圈（1是） |
| IsPublic | int | 否（可选配置） | 是否公开 |
| FilePaths | array string | 否（可选配置） | 文件或图片列表（第一张为首图） |
| PointsValues | array object | 否（可选配置） | 积分赠送配置 |
| ModuleRelationList | array object | 否（可选配置） | 关联模块列表（实体说明见活动） |
| SponsorName | string | 否 | 主办方 |
| CoSponsorName | string | 否 | 协办方 |
| SponsorDataRangeSysNo| int| 否 | 主办方ID |
| ObjectFileList| array File| 否（可选配置） | 附件 |


#### PointsValues说明 {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PointsConfigSysNo | int | 是 | 积分配置系统编码 |
| PointsValue | int | 是 | 积分值 |

#### File说明 {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FileTitle| string| 是 | 文件名称 |
| FilePath| string| 是 | 文件地址 |

#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| NewsSysNo | int | 是 | 系统编码 |





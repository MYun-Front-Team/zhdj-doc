# 修改 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新闻模块-修改

_**【应用场景】**_

新闻模块-修改

_**【接口地址】**_

[http://ip:port/NewsAction/](http://ip:port/HMAction/River/AddRiver)[News](http://ip:port/HMAction/River/AddRiver)[/E](http://ip:port/HMAction/River/AddRiver)dit[News](http://ip:port/HMAction/River/AddRiver)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| NewsSysNo | int | 是 | 新闻系统编码 |
| NewsTitle | string | 是 | 标题 |
| NewsContent | string | 是 | 内容 |
| Remark | string | 否（可选配置） | 备注 |
| IsNeedMoments | int | 否（可选配置） | 是否需要关联朋友圈（1是） |
| IsPublic | int | 否（可选配置） | 是否公开 |
| FilePaths | array string | 否（可选配置） | 文件或图片列表（第一张为首图） |
| PointsValues | array object | 否（可选配置） | 积分赠送配置 |
| ObjectFileList| array File| 否（可选配置） | 附件 |

#### File说明 {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FileTitle| string| 是 | 文件名称 |
| FilePath| string| 是 | 文件地址 |






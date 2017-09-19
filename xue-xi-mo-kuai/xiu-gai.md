# 修改 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

学习模块-修改

_**【应用场景】**_

修改。

_**【接口地址】**_

[http://ip:port/StudyAction/](http://ip:port/HMAction/River/AddRiver)[Study](http://ip:port/HMAction/River/AddRiver)[/E](http://ip:port/HMAction/River/AddRiver)dit[Study](http://ip:port/HMAction/River/AddRiver)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudySysNo | int | 是 | 系统编码 |
| StudyTitle | string | 是 | 标题 |
| StudyContent | string | 是 | 内容 |
| StudyStartTime | string | 是 | 学习开始时间 |
| StudyEndTime | string | 是 | 学习结束时间 |
| Remark | string | 否（可选配置） | 备注 |
| IsNeedMoments | int | 否（可选配置） | 是否需要关联朋友圈（1是） |
| FilePaths | array string | 否（可选配置） | 文件或图片列表（第一张为首图） |
| PointsValues | array object | 否（可选配置） | 积分赠送配置 |

####  {#应答数据-}




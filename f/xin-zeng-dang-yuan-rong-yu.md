# 新增荣誉 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增荣誉

_**【应用场景】**_

新增荣誉

_**【接口地址】**_

[http://ip:port/UMAction/Honor/Add](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)Honor

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 是 | 来源系统编码 |
| HonorTime | string | 是 | 荣誉获得日期 |
| HonorTitle | string | 是 | 荣誉抬头 |
| HonorContent | string | 是 | 荣誉说明 |
| Remark | string | 否 | 备注 |
| IsDefault | int | 否 | 是否默认 |
| FilePathList | int | 否 | 文件或图片Path列表（第一张为首图） |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| HonorSysNo | int | 是 | 荣誉系统编码 |

####  {#应答数据-（巡河记录数组）}




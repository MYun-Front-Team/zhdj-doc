# 获取下载文件列表

##### _【功能说明】_ {#【功能说明】}

获取下载文件列表

_**【应用场景】**_

获取下载文件列表

_**【接口地址】**_

http://ip:port/UMQuery/DownLoad/GetDownLoadList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| OrganizationSysNo | int | 是 | 组织编码 |

> #### _应答数据 （数组）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DownSysNo | int | 是 | 系统编码 |
| OrganizationSysNo | int | 是 | 组织编码 |
| DataRangeSysNo| int | 是 | 数据范围树 |
| FileName| string | 是 | 文件名称 |
| FilePath | string | 是 | 文件路径 |
| Remark | string | 是 | 备注 |
| DownStatus| int | 是 |文件状态0生成中，10生成完毕，11生成失败 |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceType | int | 否 |来源类型 |
| ModuleSourceClass |int| 否| 来源分类 |
| ModuleSourceSysNo | int |否 | 来源系统编码 |


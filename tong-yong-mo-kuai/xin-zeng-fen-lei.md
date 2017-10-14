# 新增分类 {#获取河长详情}

##### _【功能说明】_ {#【功能说明】}

新增分类

_**【应用场景】**_

新增分类，当只传入“CategoryTreeName”时，表示新增类别树（不存在），否则，表示在该树下，新增类别。

_**【接口地址】**_

[http://ip:port/UMAction/Category/AddC](http://ip:port/HMQuery/RiverMaster/GetRiverMasterByRiverMasterSysNo)ategory

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块系统编码（枚举） |
| ModuleSourceType | int | 否 | 模块类型（枚举） |
| CategoryTreeName | string | 是 | 类别树名称 |
| CategoryFatherSysNo | int | 否 | 类别父级主键 |
| CategoryCode | string | 否 | 类别代码 |
| CategoryName | string | 否 | 类别名称 |
| FilePathList | array string | 否 | 文件图片Path路径 |
| SortNo | int | 否 | 排序 |
| IcoImgType | int | 否 | 图片风格 |
| IcoFontType | int | 否 | 文字风格 |

> #### 应答数据 {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SysNo | int | 是 | 系统编码 |




# 修改分类 {#获取河长详情}

##### _【功能说明】_ {#【功能说明】}

修改分类

_**【应用场景】**_

修改分类

_**【接口地址】**_

[http://ip:port/UMAction/Category/EditC](http://ip:port/HMQuery/RiverMaster/GetRiverMasterByRiverMasterSysNo)ategory

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CategorySysNo | int | 是 | 系统编码 |
| CategoryCode | string | 否 | 类别代码 |
| CategoryName | string | 否 | 类别名称 |
| FilePathList | array string | 否 | 文件图片Path路径 |
| SortNo | int | 否 | 排序 |
| IcoImgType | int | 否 | 图片风格 |
| IcoFontType | int | 否 | 文字风格 |

> #### 应答数据 {#应答数据-}




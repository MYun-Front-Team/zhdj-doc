# 获取分类列表 {#获取河长详情}

##### _【功能说明】_ {#【功能说明】}

获取分类列表

_**【应用场景】**_

获取分类列表

_**【接口地址】**_

[http://ip:port/UMQuery/Category/GetC](http://ip:port/HMQuery/RiverMaster/GetRiverMasterByRiverMasterSysNo)ategorys

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块系统编码（枚举） |
| ModuleSourceType | int | 否 | 模块类型（枚举） |
| CategoryTreeName | int | 是 | 类别树名称 |
| CategoryFatherSysNo | int | 否 | 类别父级主键（传0表示获取根类别） |
| IsShowBranch | int | 否 | 是否显示分支（递归树状） |

> #### 应答数据 {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| CategorySysNo | int | 是 | 系统编码 |
| CategoryFatherSysNo | int | 否 | 类别父级主键 |
| CategoryCode | string | 否 | 类别代码 |
| CategoryName | string | 否 | 类别名称 |
| SortNo | int | 否 | 排序 |
| Remark | string | 否 | 备注 |
| FileUrlList | array string | 否 | 文件图片url列表 |
| Categorys | array object | 否 | 类别列表 |




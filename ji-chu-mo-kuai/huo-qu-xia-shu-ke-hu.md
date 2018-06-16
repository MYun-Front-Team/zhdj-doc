# 获取角色权限列表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取角色权限列表

_**【应用场景】**_

获取角色权限列表

_**【接口地址】**_

http://ip:port/BasicQuery/Basic/GetSonPersons

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员系统编码 |

> #### 应答数据 （PageResponseBase）【38000100】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员系统编码 |
| PersonName | string | 否 | 昵称 |
| RealName | string | 否 | 真实姓名 |
| CellPhoneNo | string | 否 | 手机 |
| CreateTime| string | 否 | 创建时间 |
| CustomerLevelName| string | 否 | 客户等级 |
| CustomerLevelSysNo| int| 否 | 客户等级编码 |
| CustomerSonCount| int| 否 | 下级人数 |
| FileUrlList | array string | 否 | 头像图片列表 |





# 获取人员基本信息 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取人员基本信息

_**【应用场景】**_

获取人员基本信息

注：通过User来判断请求参数中的PersonSysNo是否是好友关系。

_**【接口地址】**_

[http://ip:port/ChatQuery/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)Chat[/G](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)etMyPersonFriend

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员系统编码 |
| BizCompanyCode | int | 否 | 项目号 |
| Limit | object | 否 | 限制条件 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| GroupStatistic | object | 否 | 统计字段 |
| Person | object | 是 | 人员实体对象 |

#### Person说明_ （简要，需要全部字段请调用“获取个人信息”接口）_ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员系统编码 |
| PersonName | string | 否 | 昵称 |
| RealName | string | 否 | 真实姓名 |
| CellPhoneNo | string | 否 | 手机 |
| UserGender | int | 否 | 性别：1男，2女 |
| BirthDay | string | 否 | 生日 |
| PersonAge | int | 否 | 年龄 |
| PCDCode | string | 否 | 省市区 |
| PCDDescription | string | 否 | 省市区 |
| ContractAddress | string | 否 | 地址 |
| ~~Post~~ | ~~string~~ | ~~否~~ | ~~工作岗位~~ |
| FileUrlList | array string | 否 | 图片列表（首图为头像） |




# 新增个人联系方式 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

新增个人联系方式

_**【应用场景】**_

新增个人联系方式

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/A](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ddPersonContact

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员编码（如果不传则获取UserSysNo对应的Person） |
| ContactType | int | 否 | 联系类型：0手机，1邮箱，2社交账号，3网站 |
| ContactClassSysNo | int | 否 | 联系类型分类编码 |
| ContactWay | string | 是 | 联系方式 |
| IsDefault | int | 否 | 是否默认联系方式 |
| Remark | string | 否 | 备注 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ContactSysNo | int | 是 | 系统编码 |




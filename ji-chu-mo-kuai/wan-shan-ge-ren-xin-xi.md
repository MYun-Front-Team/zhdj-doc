# 完善个人信息 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

完善个人信息

_**【应用场景】**_

完善个人信息

_**【接口地址】**_

[http://ip:port/BasicAction/](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[Basic](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)[/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditPerson

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 否 | 人员编码（如果不传则修改UserSysNo对应的Person） |
| PersonName | string | 否 | 昵称 |
| RealName | string | 否 | 真实姓名 |
| UserGender | int | 否 | 性别：1男，2女 |
| BirthDay | string | 否 | 生日 |
| PCDCode | string | 否 | 省市区 |
| PCDDescription | string | 否 | 省市区 |
| ContractAddress | string | 否 | 地址 |
| Post | string | 否 | 工作岗位 |
| IDCard | string | 否 | 身份证 |
| Nation | string | 否 | 民族 |
| Origin | string | 否 | 籍贯 |
| Education | int | 否 | 学历：0未知,1小学,2初中,3中转,4高中,5专科,6本科,7硕士,8博士 |
| FileUrlList | array string | 否 | 图片列表（首图为头像） |




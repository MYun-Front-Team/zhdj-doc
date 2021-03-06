# 新增人员

##### _【功能说明】_ {#【功能说明】}

新增人员

_**【应用场景】**_

新增人员

_**【接口地址】**_

[http://ip:port/BasicAction/Basic/AddPerson](http://ip:port/BasicAction/Basic/AddPerson)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonName | string | 否 | 昵称 |
| RealName | string | 否 | 真实姓名 |
| UserGender | int | 否 | 性别：1男，2女 |
| BirthDay | string | 否 | 生日 |
| PCDCode | string | 否 | 省市区 |
| PCDDescription | string | 否 | 省市区 |
| ContractAddress | string | 否 | 地址 |
| CompanyName | string | 否 | 公司名称 |
| Post | string | 否 | 工作岗位 |
| IDCard | string | 否 | 身份证 |
| Nation | string | 否 | 民族 |
| Origin | string | 否 | 籍贯 |
| Education | int | 否 | 学历：0未知,1小学,2初中,3中转,4高中,5专科,6本科,7硕士,8博士,9其它 |
| FileUrlList | array string | 否 | 图片列表（首图为头像） |
| PersonProfile | string | 否 | 个人简介 |
| WorkingDate | string | 否 | 参加工作日期 |
| Propertys | array object | 否 | 人员属性列表（见通用属性说明） |
| PrivacyPropertys | array object | 否 | 隐私属性列表 |
| TagSysNoList | array int | 否 | 标签列表 |
| IfVerify | int | 否 | 是否要连接三方查证身份证合法性 |
| FileLifePathList | array string | 否 | 生活照图片列表 |
| BloodType | string | 否 | 血型 |
| Anaphylaxis | string | 否 | 过敏史 |
| Hobby | string | 否 | 爱好 |
| Remark | string | 否 | 备注 |
| IDCardType | int | 否 | 证件类型 |
| NeedPartTimeJob | int | 否 | 是否屏蔽推送兼职（0正常，1屏蔽） |
| CellPhoneNo | string | 否 | 手机号 |
| OrganizationSysNo | int | 否 | 所属医院组织编码 |
| OrganizationTypeList | array\[int\] | 否 | 组织类型 医生组织类型 |
| DataRangeSysNoList | array\[int\] | 否 | 数据范围 |




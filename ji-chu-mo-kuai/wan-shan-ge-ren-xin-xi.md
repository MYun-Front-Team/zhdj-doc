# 完善个人信息 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

完善个人信息

_**【应用场景】**_

完善个人信息

注：人员属性列表参数不提供则不修改，提供但列表数量为0则删除。

_**【接口地址】**_

[http://ip:port/BasicAction/Basic/EditPerson](http://ip:port/BasicAction/Basic/EditPerson)

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
| CompanyName | string | 否 | 公司名称 |
| Post | string | 否 | 工作岗位 |
| IDCard | string | 否 | 身份证 |
| Nation | string | 否 | 民族 |
| Origin | string | 否 | 籍贯 |
| Education | int | 否 | 学历：0未知,1小学,2初中,3中转,4高中,5专科,6本科,7硕士,8博士,9其它，20硕士生班，21中央党校研究生，22省（区、市）委党校研究生，23大学，24第二学士学位班，25中央党校大学，26省（区、市）委党校大学，27中央党校大专，28省（区、市）委党校大专，29职业高中，30技术学校 |
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
| DoctorPersonInvitaionCode | string | 否 | 医生邀请码 |
| Salesman | string | 否 | 业务员 |
| OrganizationSysNo | int | 否 | 组织编码（用于修改T\_RM\_OrgPersonRelation的PostSysNo） |
| PostSysNo | int | 否 | 职位编码（端自定义） |
| PCDDataRangeSysNoList | array\[int\] | 否 | 负责区域系统编码列表 |




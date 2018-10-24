# 获取个人信息 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

获取个人信息

_**【应用场景】**_

获取个人信息

_**【接口地址】**_

http://ip:port/BasicQuery/Basic/GetPersonBySysNo

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员编码（如果不传则获取UserSysNo对应的Person） |
| Longitude| decimal| 否 | Longitude |
| Latitude| decimal| 否 | Latitude |
| Limit | object | 否 | 限制条件 |

#### Limit说明_ _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsShowPropertys | int | 否 | 是否显示人员属性列表 |
| IsShowPrivacyPropertys | int | 否 | 是否显示隐私属性列表 |
| IsShowTagList | int | 否 | 是否显示标签列表 |
| IsShowFatherPerson | int | 否 | 是否显示推荐人 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员系统编码 |
| PersonName | string | 否 | 昵称 |
| RealName | string | 否 | 真实姓名 |
| CellPhoneNo | string | 否 | 手机 |
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
| FileUrlList | array string | 否 | 头像图片列表 |
| PersonIDPhotoUrlList | array string | 否 | 证件照图片列表 |
| PersonProfile | string | 否 | 个人简介 |
| WorkingDate | string | 否 | 参加工作日期 |
| Propertys | array object | 否 | 人员属性列表（见通用属性说明） |
| PrivacyPropertys | array object | 否 | 隐私属性列表 |
| LoginIDStatus | int | 否 | 账号类型：0正常，1无账号，2未激活 |
| PersonIDCardUrlList | array string | 否 | 身份证图片列表 |
| ResidencePermitUrlList | array string | 否 | 居住证图片列表 |
| TagList | array object | 否 | 标签列表 |
| FatherPersonName | string | 否 | 推荐人名字 |
| FatherPersonSysNo | int | 否 | 推荐人编码 |
| FileLifeUrlList | array string | 否 | 生活照图片列表 |
| Longitude| decimal| 否 | Longitude |
| Latitude| decimal| 否 | Latitude |
| Distance| decimal\(18,2\) | 否 | 距离店铺距离 |
| BloodType| string| 否 | 血型|
| Anaphylaxis| string| 否 |过敏史|
| Hobby| string| 否 |爱好|
| Remark| string| 否 |备注|
| InSchoolStatus| int | 否 | 在校学生状态（0不明 1是 2不是） |
| IDCardType | int| 否 | 证件类型|
| NeedPartTimeJob| int | 否 | 是否屏蔽推送兼职（0正常，1屏蔽） |
| DoctorPersonSysNo| int | 否 | 医生编码 |
| Salesman | string| 否 | 业务员 |



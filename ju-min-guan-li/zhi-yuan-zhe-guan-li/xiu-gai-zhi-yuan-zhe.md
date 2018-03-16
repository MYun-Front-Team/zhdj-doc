# 修改志愿者 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

修改志愿者

_**【应用场景】**_

修改志愿者

注：只有审核失败时，传入VolunteerStatus=1才有效。

_**【接口地址】**_

[http://ip:port/ResidentAction/Volunteer/E](http://ip:port/HMQuery/PatrolRiver/GetPatrolRivers)ditVolunteer

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| VolunteerSysNo | int | 是 | 系统编码 |
| OtherSpecialty | string | 否 | 其它特长与爱好 |
| VolunteerExperience | string | 否 | 义工或社工经历 |
| BuddhistExperience | string | 否 | 佛教经历 |
| Remark | string | 否 | 备注 |
| SpecialtyClassSysNoList | array int | 否 | 特长与爱好编码列表（分类） |
| Longitude | decimal\(18,10\) | 否 | 经度 |
| Latitude | decimal\(18,10\) | 否 | 纬度 |
| VolunteerStatus | int | 否 | 志愿者状态：1待审核 |
| EditPerson | object | 否 | 人员信息 |
| EditResident | object | 否 | 居民信息 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




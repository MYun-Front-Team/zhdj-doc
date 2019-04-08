# 获取社区干部报表

_**【接口地址】**_

http://ip:port/PartyQuery/Party/GetCadreReport

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 区级id |


#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 区级id |
| DataRangeName | string | 是 | 区名称 |
| StreetNum | int | 是 | 镇街道数量 |
| VillageNum | int | 是 | 村社区数量 |
| CadreNum | int | 是 | 干部总数|
| InnerPartyStatusList | array object | 是 | 政治面貌列表 |
| EducationList | array object | 是 | 学历列表 |
| GenderList | array object | 是 | 性别列表 |
| AgeList | array object | 是 | 年龄列表 |
| StreetList | array object | 是 | 镇街道列表 |


| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Key | string | 是 | 键名称 |
| Value | decimal | 是 | 值 |



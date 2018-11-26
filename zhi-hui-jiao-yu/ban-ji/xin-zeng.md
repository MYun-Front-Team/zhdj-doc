# 新增 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

新增

_**【应用场景】**_

注：1、同数据范围+同年级 下的班级名称不能重复；

2、班级与教师关系类型为“班主任”或“副班主任”则关系设置为默认值，后期用住查询；

3、通过父级编码先维护数据范围树结构；

_**【接口地址】**_

[http://ip:port/EduAction/Class/Add](http://ip:port/HMAction/River/AddRiver)Class

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeFatherSysNo | int | 是 | 父级数据范围枝叶编码 |
| ~~GradeSysNo~~ | ~~int~~ | ~~是~~ | ~~年级系统编码~~ |
| ClassName | string | 是 | 班级名称 |
| ClassMotto | string | 否（可选配置） | 班训 |
| HeadMasterWord | string | 否（可选配置） | 班主任寄语 |
| AddClassTeacherList | array object | 否（可选配置） | 新增班级教师列表 |
| AddCollectivePhotoList | array string | 否（可选配置） | 新增集体照列表 |
| AddClassBannerList | array string | 否（可选配置） | 新增班旗列表 |
| SortNo| int | 是 | 排序|


#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ClassSysNo | int | 是 | 系统编码 |

#### AddClassTeacher说明 {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ClassTeacherType | int | 是 | 类型： 1班主任，2副班主任，99教师 |
| TeacherSysNo | int | 是 | 教师系统编码 |




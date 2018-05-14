# 修改 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改

_**【应用场景】**_

注：1、同数据范围+同年级 下的班级名称不能重复；

2、班级与教师关系类型为“班主任”或“副班主任”则关系设置为默认值，后期用住查询；

3、同一班级 不允许存在多个“班主任”或“副班主任”；

_**【接口地址】**_

[http://ip:port/EduAction/Class/E](http://ip:port/HMAction/River/AddRiver)ditClass

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ClassSysNo | int | 是 | 数据范围枝叶编码 |
| ~~GradeSysNo~~ | ~~int~~ | ~~否~~ | ~~年级系统编码~~ |
| ClassName | string | 否 | 班级名称 |
| ClassMotto | string | 否 | 班训 |
| HeadMasterWord | string | 否 | 班主任寄语 |
| EditClassTeacherList | array object | 否 | 修改班级教师列表 |

#### _应答数据_ {#应答数据-}

#### EditClassTeacher说明 {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SysNo | int | 是 | 系统编码 |
| ClassTeacherType | int | 是 | 类型： 1班主任，2副班主任，99教师 |
| TeacherSysNo | int | 是 | 教师系统编码 |




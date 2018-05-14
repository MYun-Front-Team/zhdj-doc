# 设置班级图片 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

设置班级图片

_**【应用场景】**_

设置班级图片

注：该接口兼容图片新增、修改、删除功能；

_**【接口地址】**_

[http://ip:port/EduAction/](http://ip:port/HMAction/River/AddRiver)Class[/S](http://ip:port/HMAction/River/AddRiver)etClassImgList

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ClassSysNo | int | 是 | 班级系统编码 |
| CollectivePhotoPathList | array string | 否 | 集体照Path列表（第一张为首图） |
| ClassBannerPathList | array string | 否 | 班旗Path列表（第一张为首图） |

> #### 应答_数据_ {#请求数据}




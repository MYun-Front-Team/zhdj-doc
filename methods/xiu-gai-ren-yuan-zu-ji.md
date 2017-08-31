# 修改人员足迹 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

修改人员足迹

_**【应用场景】**_

修改人员足迹

_**【接口地址】**_

[http://ip:port/UMAction/Info/E](http://ip:port/HMAction/River/AddRiver)ditInfoPersonFootPrint

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| FootPrintSysNo | int | 是 | 人员足迹系统编码 |
| Name | string | 否 | 姓名 |
| CellPhoneNo | string | 否 | 手机 |
| PersonStatus | int | 是 | 状态：0报名/阅读/分享,1审核/确认，10签到/完成，11删除/请假 |
| IsEnable | int | 否 | 是否有效 |
| SignCount | int | 否 | 足迹数量 |
| SignTime | string | 否 | 足迹时间 |
| SignPlace | string | 否 | 足迹地点（签到/活动地） |
| SignJson | string | 否 | 端自定义字段（原样返回） |
| Reason | string | 否 | 原因 |
| Remark | string | 否 | 备注 |
| FilePaths | array string | 否 | 文件图片列表 |
| SourceOperateType | int | 否 | 来源操作类型：0新增，1查看，2回复，3审核，4上传，5下载，6签到，10完结（如传该参数，则判断是否需要赠送积分） |




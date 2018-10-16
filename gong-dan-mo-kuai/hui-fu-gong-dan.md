# 回复工单

##### _【功能说明】_ {#【功能说明】}

回复工单

_**【应用场景】**_

回复工单

注：该接口支持2种场景：

1、工单提交后，未选中处理人，则可见该工单的相关人员可以流转指派；（某部门的谁指派给某部门的谁）

2、相关人员回复给提交人；

_**【接口地址】**_

http://ip:port/WorkAction/Work/ReplyWork

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WorkSysNo | int | 是 | 系统编码 |
| ReplyContent | string | 是 | 回复内容 |
| ReplyTime | string | 否 | 回复时间 |
| ToDataRangeSysNo | int | 否 | 流转数据范围系统编码 |
| ToPersonSysNo | int | 否 | 流转人员系统编码 |
| ReplyFilePathList | array string | 否（可选配置） | 文件或图片Path列表（第一张为首图） |


#### _应答数据_ {#应答数据-}




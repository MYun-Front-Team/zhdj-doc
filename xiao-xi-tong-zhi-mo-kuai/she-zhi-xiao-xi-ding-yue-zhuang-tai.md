# 设置消息订阅状态

##### _【功能说明】_ {#【功能说明】}

设置消息订阅状态（不设置的话均订阅）

_**【应用场景】**_
设置消息订阅状态（不设置的话均订阅）


_**【接口地址】**_

http://ip:port/MessageAction/Message/SetMessageConfigSubStatus

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 否 | 模块编码 |
| ModuleSourceType | int | 否 | 来源类型 |
| ModuleSourceClass | int | 否 | 来源分类 |
| ModuleSourceSysNo | int | 否 | 来源系统编码 |
| OperateType | int | 否 | 操作类型 |
| BizCompanyCode | int | 是 | BizCompanyCode |
| SubStatus | int | 是| 订阅状态：0取消订阅，1订阅 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}




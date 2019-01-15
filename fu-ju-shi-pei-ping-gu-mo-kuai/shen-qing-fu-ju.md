# 获取申请详情

_**【接口地址】**_

http://ip:port/FJAction/Adaption/AddApply

> #### _请求数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ApplyPersonSysNo | int | 是 | 申请人编码 |
| PersonSysNo | int | 是 | 人员id |
| AssistantType | int | 是 | 申请辅助器具类别id |
| ApplyRemark | string | 是 | 申请辅助器具说明 |
| SubsidyTypeSysNoList | array int | 是 | 符合补贴人群类别列表 |

> #### _应答数据_

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ApplySysNo | int | 是 | 申请id |

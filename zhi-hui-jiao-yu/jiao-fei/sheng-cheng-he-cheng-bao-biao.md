# 生成禾城报表 {#获取河长巡河记录}

##### _【功能说明】_ {#【功能说明】}

生成禾城报表

_**【应用场景】**_

生成禾城报表

注：只有审核通过且未开始缴费状态的记录才能生成报表。

导出到通用文件中的Excel下载功能区；



_**【接口地址】**_

http://ip:port/StudentFeeQuery/StudentFee/GetStudentFeePersons

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentFeeSysNo | int | 是 | 缴费编码 |
| PersonStatusList|array int | 是 | 状态：0未缴，1部分, 10已缴，11弃缴 |
| DataRangeSysNoList | int | 否 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| DataRangeSysNoList | int | 否 | 数据范围树枝叶编码列表 |
| KeyWord | string | 否 | 关键字搜索（名称） |





> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentFeePersonSysNo | int | 是 | 缴费系统明细编码 |
| DataRangeCode| string| 是 | 委托编号|
| BankFeeCode| string| 是 | 费用类型|
| SubPaidClassCode | string| 是 | 子费种编码\(通用类\) |
| SubPaidClassName | string | 是 | 子费种名称 |
| PersonName| string| 是 | 学生名称 |
| DataRanges| array[DataRange]| 是 | 班级-年级-学校数组 |
| PayAbleAmount| decimal| 是 | 应缴金额 |
| Remark| string| 是 | 备注 |
|PersonStatus|int | 是 |状态：0未缴，1部分, 10已缴，11弃缴 |
|Reason|string | 是 |状原因 |
|PaidTime|string | 是 |缴费时间 |
| PaidAmount| decimal| 是 | 已缴金额 |
| ConfirmStatus | int | 是 | 确认状态：0待确认，10已确认|







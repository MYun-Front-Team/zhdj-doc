# 生成禾城报表汇总

##### _【功能说明】_ {#【功能说明】}

生成禾城报表汇总

_**【应用场景】**_

生成禾城报表汇总

注：只有审核通过且未开始缴费状态的记录才能生成报表。

导出到通用文件中的Excel下载功能区；



_**【接口地址】**_

http://ip:port/StudentFeeQuery/StudentFee/GetStudentFeePersonTotal

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| StudentFeeSysNo | int | 是 | 缴费编码 |
| DataRangeSysNoList | int | 否 | 数据范围树枝叶编码列表 |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |






> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PayAbleTotalAmount | decimal\(18,2\) | 否 | 总金额 |
| PersonTotalCount | int | 否 | 待缴总人数 |
| TotalAmount | decimal\(18,2\) | 否 | 总金额 |
| ExemptCount | int | 否 |列外人数 |











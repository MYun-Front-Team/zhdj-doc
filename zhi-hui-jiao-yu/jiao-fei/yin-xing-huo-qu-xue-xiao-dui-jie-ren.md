#银行设置学校对接人

##### _【功能说明】_ {#【功能说明】}

银行设置学校对接人

_**【应用场景】**_

银行设置学校对接人



_**【接口地址】**_

http://ip:port/StudentFeeQuery/StudentFee/GetDataRangeFeePerson
> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 数据范围树枝叶编码|


> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 数据范围树枝叶编码|
| FeePersonName| string| 是 |对接人名称|
| FeePersonCellPhone| string| 是 |对接人电话|
| PaymentMethod|List[int] | 是 | 允许的支付方式 0线下 1线上|
| PaymentType | int | 是 | 对接的银行（9禾商行，8工行E支付）|






获取银行对接人列表

##### _【功能说明】_ {#【功能说明】}
获取银行对接人列表

_**【应用场景】**_

获取银行对接人列表


_**【接口地址】**_

http://ip:port/StudentFeeQuery/StudentFee/GetDataRangeFeePersonList
> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| IsBranch | int | 否 | 是否枝叶，向下兼容查询：0查树，1查枝叶 |
| DataRangeSysNoList |array[int] | 否 | 数据范围树枝叶编码列表 |
| KeyWord| string| 是 |对接人名称|
| ModuleSourceTypeList| array[int]| 否 |模块类型|




> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNo | int | 是 | 数据范围树枝叶编码|
| FeePersonName| string| 是 |对接人名称|
| FeePersonCellPhone| string| 是 |对接人电话|
| PaymentMethod|List[int] | 是 | 允许的支付方式 0线下 1线上|
| PaymentType | int | 是 | 对接的银行（9禾商行，8工行E支付）|
| ModuleSourceType| int | 否 |模块类型|












# 新增商品 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/EqmAction/Equipment/AddEqmProduct](http://ip:port/EqmQuery/Equipment/GetEqmProductBySysNo)

> #### _请求数据_ {#请求数据}



| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ProductGroupName | string | 是 | 商品名称 |
| ImgList | array string | 否 | 图片列表 |
| SalePrice | decimal\(18,2\) | 是 | 销售价格 |
| EquipmentTypeSysNoList | array int | 是 | 适用设备类型编码列表 |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}



| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| Body | int | 是 | 商品编码 |




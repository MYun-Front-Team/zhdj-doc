# 获取异常名单详情 {#获取河长巡河记录}

_**【接口地址】**_

[http://ip:port/VDQuery/Detect/GetAbnormalBySysNo](http://ip:port/VDQuery/Detect/GetAbnormalBySysNo)

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AbnormalSysNo | int | 否 | 异常名单id |

> #### _应答数据 _ {#应答数据-（巡河记录数组）}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| AbnormalSysNo | int | 是 | 异常名单id |
| OrganizationSysNo | int | 是 | 检测站组织名称 |
| dsName | string | 是 | 检测机构名称 |
| vehicleType | string | 是 | 挂车，牵引车，客车，货车，专项作业车，其他 |
| vehicleTypeName | string | 是 | 车辆类型 |
| detectDate | datetime | 是 | 检测日期 |
| vehicleNo | string | 是 | 车牌号码 |
| plateColorCode | string | 是 | 车牌颜色 |
| vehicleBrandModel | string | 是 | 品牌型号 |
| remark | string | 是 | 备注 |
| LastModifyTime | datetime | 是 | 更新时间 |




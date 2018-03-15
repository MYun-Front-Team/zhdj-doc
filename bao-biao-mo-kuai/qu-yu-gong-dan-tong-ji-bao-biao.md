# 工单报表 {#获取河长巡河记录}

#### 页面编号枚举说明 {#请求数据}

| 页编码 | 模块说明 | 页面说明 |
| :--- | :--- | :--- |
| 24000100 | 工单报表 | 按区域维度 |



> #### 请求数据（PageRequestData）_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| WorkType| int | 是 | 工单类型 |
> #### 应答数据 （PageResponseBase）【24000100】

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeName| string | 是 | 地区 |
| DataRangeSysNo| int | 是 | DataRangeSysNo |
| WorkCount| int | 是 | 数量|



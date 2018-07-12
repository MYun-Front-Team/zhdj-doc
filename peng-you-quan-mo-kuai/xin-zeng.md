# 新增 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

朋友圈模块-新增

_**【应用场景】**_

朋友圈模块-新增。

注：MomentsPerson实体是发布时，发布人所在地的定位地址，该功能是可选配置。

ModuleRelationList如参加活动模块后，可发布活动的相关朋友圈，形成关联。

积分备注：新增动作（枚举=15）预埋积分赠送逻辑。（如果是其它模块关联新增（枚举=11），则赠送逻辑依照该模块的配置）

_**【接口地址】**_

[http://ip:port/MomentsAction/Moments/Add](http://ip:port/HMAction/River/AddRiver)Moments

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| DataRangeSysNoList | array int | 是 | 数据范围枝叶编码列表（必须在不同的树中的枝叶） |
| MomentsType | int | 否（可选配置） | 类型（枚举） |
| MomentsClassSysNo | int | 否（可选配置） | 类型分类系统编码（类别树） |
| PersonPost | string | 否 | 岗位（业务模块冗余） |
| PersonDepartment | string | 否 | 部门（业务模块冗余） |
| MomentsTitle | string | 否 | 标题 |
| MomentsContent | string | 是 | 内容 |
| FilePaths | array string | 否 | 文件或图片列表（第一张为首图） |
| MomentsPerson | object | 否（可选配置） | 发布时定位自己位置 |
| ModuleRelationList | array object | 否（可选配置） | 关联模块列表（实体说明见活动） |
| IsShowInMoments | int | 否 | 是否显示在朋友圈：0否，1是（当有关联模块时该字段有效） |


#### _应答数据_ {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| MomentsSysNo | int | 是 | 系统编码 |

#### MomentsPerson说明 {#应答数据-}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| SignPlace | string | 是 | 足迹地点 |
| Longitude | decimal | 否 | 经度 |
| Latitude | decimal | 否 | 纬度 |




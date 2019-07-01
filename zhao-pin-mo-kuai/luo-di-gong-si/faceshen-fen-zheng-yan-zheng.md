#Face++身份证验证
##### _【功能说明】_ {#【功能说明】}

Face++身份证验证

_**【应用场景】**_

Face++身份证验证


_**【接口地址】**_

http://ip:port/RecruitAction/MyBank/OcrIDCard

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PersonSysNo | int | 是 | 人员系统编码 |
| ImageBase64| string | 是 | 图片的base64数据|
| ImageUrl| string| 否 | 图片Url |


> #### _返回数据

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| cards| array[Card] | 是 | 检测出证件的数组 注：如果没有检测出证件则为空数组 |
| error_message| string | 是 |当请求失败时才会返回此字符串,否则此字段不存在|

> #### _返回数据Card

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| type| int | 是 | 证件类型，返回1，代表是身份证 |
| address| string | 是 | 住址|
| birthday| string| 是 | 生日，格式为YYYY-MM-DD |
| gender| string| 否 | 性别（男/女） |
| id_card_number| string| 否 |身份证号|
| name| string| 否 | 	姓名 |
| race| string| 否 | 民族（汉字）|
| side| string| 否 | 表示身份证的国徽面或人像面。返回值为：front: 人像面 back: 国徽面 |
| issued_by| string| 否 | 签发机关 |
| valid_date| string| 否 | 有效日期，返回值有两种格式，一个16位长度的字符串：YYYY.MM.DD-YYYY.MM.DD 或是：YYYY.MM.DD-长期|
| legality| object| 否 | 身份证照片的合法性检查结果，:{\"ID Photo\":1.0,\"Temporary ID Photo\":0.0,\"Photocopy\":0.0,\"Screen\":0.0,\"Edited\":0.0} |




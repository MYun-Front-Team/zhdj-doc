# 创建在线支付 {#新增河流}

##### _【功能说明】_ {#【功能说明】}

创建在线支付

_**【应用场景】**_

创建在线支付

注：1、在线支付支持的有：0余额，1支付宝，2微信，3银联，4线下支付，5刷卡支付，6积分支付,7联动支付，8工行E支付，9禾商行

2、当IsNeedBalance=1时，先扣出全部可用余额后，在把剩余不足的钱用第三方付款；

订单支付：ModuleSysNo=23000，ModuleSourceSysNo=订单编码，其它=0

商家会员支付：ModuleSysNo=27000，ModuleSourceSysNo=商家编码，其它=0

3、刷卡支付时，CardNo和CardKey必填，需验证卡的秘密正确后，找到卡所属组织，然后进行钱包支付；

4、充值功能（有会员卡）：直充钱包ModuleSysNo=26000，ModuleSourceType=26001，ModuleSourceClass=1，ModuleSourceSysNo=充值系统编码；

5、保证金功能：直充钱包ModuleSysNo=26000，ModuleSourceType=26007，ModuleSourceClass=0，ModuleSourceSysNo=保证金系统编码；

6、会员费功能：直充钱包ModuleSysNo=26000，ModuleSourceType=26008，ModuleSourceClass=0，ModuleSourceSysNo=会员费系统编码；

7、代理费功能：直充钱包ModuleSysNo=26000，ModuleSourceType=26010，ModuleSourceClass=0，ModuleSourceSysNo=代理费系统编码；

8、充值功能（无会员卡）：直充钱包ModuleSysNo=26000，ModuleSourceType=26011，ModuleSourceClass=0，ModuleSourceSysNo=充值系统编码；

8、充值积分：直充钱包ModuleSysNo=3000，ModuleSourceType=304，ModuleSourceClass=0，ModuleSourceSysNo=待支付积分流水编码；

10、园区费用支付ModuleSysNo=35000，ModuleSourceType=智慧园区-费用类型（35001，35002……），ModuleSourceClass=0，ModuleSourceSysNo=PayFeeSysNo（缴费流水编码）；

11、党费支付ModuleSysNo=9000，ModuleSourceType=9003，ModuleSourceClass=0，ModuleSourceSysNo=FeeLogSysNo
（缴费流水编码）；

11、教育学费支付ModuleSysNo=39000，ModuleSourceType=39008，ModuleSourceClass=0，ModuleSourceSysNo=StudentFeePersonSysNo 缴费系统明细编码；



_**【接口地址】**_

http://ip:port/DealQuery/Payment/GetPaymentUrl

> #### _请求数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| ModuleSysNo | int | 是 | 模块编码 |
| ModuleSourceType | int | 是 | 模块来源类型 |
| ModuleSourceClass | int | 是 | 模块来源分类 |
| ModuleSourceSysNo | int | 是 | 模块来源系统编码 |
| PaymentSysNo | int | 否 | 支付方式系统编码 |
| IsNeedBalance | int | 否 | 是否需要先扣余额：0否，1是 |
| OpenID | string | 否 | 微信OPENID |
| CardNo | string | 否 | 卡号 |
| CardKey | string | 否 | 卡密码 |
| UnderlinePayAmount | decimal\(18,2\) | 否 | 线下支付金额 |
| ~~PaymentAmount~~ | ~~decimal\(18,2\)~~ | ~~否~~ | ~~充值金额（充值钱包时必填）~~ |

> #### 应答_数据_ {#请求数据}

| 变量名 | 类型 | 是否必须 | 描述 |
| :--- | :--- | :--- | :--- |
| PaymentUrl | string | 是 | 支付方式系统编码 |




# 微信扫码支付 WxPay

作用：商家生成订单后，扫描顾客付款二维码进行收款；

### 设计属性

#### 1、微信支付：

* ##### 活动标题

  * 类型：字符串；

  * 值：默认值：微信支付；

  * 说明：
* ##### 活动注释

  * 类型：字符串；

  * 值：

  * 说明：对活动的说明；
* ##### App Id

  * 类型：字符串；

  * 说明：微信开放平台审核通过的移动应用APPID；
* ##### 公众号Id

  * 类型：字符串；

  * 说明：微信公众平台审核通过的公众号APPID；
* ##### MchId

  * 类型：字符串；

  * 示例：DBAzure；

  * 说明：微信支付分配的商户号，需与APPID签约绑定关系；
* ##### SubAppId

  * 类型：字符串；

  * 说明：子应用APPID，可不填；
* ##### SubMchId

  * 类型：字符串；

  * 说明：子商户号，可不填；
* ##### 签名密钥

  * 类型：字符串；

  * 值：

  * 说明：签名密钥；
* ##### 交易类型

  * 类型：字符串；

  * 值：

  * 说明：可选类型：

    APP：微信App支付；

    JSAPI：微信公众号支付；

    NATIVE：微信后台系统返回链接参数code\_url，商户后台系统将code\_url值生成二维码图片，用户使用微信客户端扫码后发起支付；注意：

    code\_url有效期为2小时，过期后扫码不能再发起支付。
* ##### 订单号

  * 类型：字符串；

  * 说明：用于支付的商户订单号；
* ##### 支付金额

  * 类型：数值；

  * 示例:@0.01；

  * 说明：设置支付金额；
* ##### 备注

  * 类型：字符串；

  * 示例：测试支付订单；

  * 说明：微信支付界面的显示信息，商品信息。_**不能为空**_；
* ##### 操作员

  * 类型：字符串；

  * 示例：收银员；

  * 说明：填写操作员信息；
* ##### 支付码

  * 类型：字符串；

  * 值：示例:@barcode；

  * 说明：扫描客户付款码获取的值，通过“条码扫描”组件获取。

#### 2、调用成功：调用成功时需要执行的操作

* ##### 活动标题

  * 类型：字符串；

  * 值：默认值：调用成功；

  * 说明：
* ##### 活动注释

  * 类型：字符串；

  * 值：

  * 说明：对活动的说明；

#### 3、调用失败：调用失败时需要执行的操作

* ##### 活动标题

  * 类型：字符串；

  * 值：默认值：调用失败；

  * 说明：
* ##### 活动注释

  * 类型：字符串；

  * 值：

  * 说明：对活动的说明；

##### 回调函数参数：

* ##### payinfo-获取支付信息对象

  * 类型：对象；

  * 说明：在“调用成功”和“调用失败”中可以获取支付信息对象payinfo。支付信息对象属性JSonData对象包含“交易编号”、“订单号”、“支付金额”属性。

  * 结构：

  * ```js
    //transaction_id:交易编号；
    //OrderId：订单号；
    //TotalFee：支付金额；
    {"JSonData":{"transaction_id":
    "42000003082019……",
    "OrderId":"234123123123",
    "TotalFee":0.01},"Exception":"","State":0};
    ```



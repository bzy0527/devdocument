# 磁贴列表视图MetroNavView

---

### ![](/assets/MetroNavView.png)

### 设计属性

* ##### 对象名称

  * 类型：字符串；

  * 值：

  * 说明：自定义控件对象名；
* ##### 列表成员

  * 类型：字符串；

  * 值：

  * 说明：设置绑定数据源字段；
* ##### 标题成员

  * 类型：字符串；

  * 值：默认：Text

  * 说明：数据源ItemSource中的标题字段名；
* ##### 图片成员

  * 类型：字符串；

  * 值：默认：ImageUrl；

  * 说明：数据源ItemSource中的显示图片字段名；
* ##### 计数成员

  * 类型：字符串；

  * 值：默认：counter

  * 说明：数据源ItemSource中计数字段名；
* ##### 描述成员

  * 类型：字符串；

  * 值：默认：Description

  * 说明：数据源ItemSource中的描述信息字段名；
* ##### 项目高度

  * 类型：字符串；

  * 值：默认：160px

  * 说明：设置项目高度，默认显示160px；
* ##### 每行列数

  * 类型：数值；

  * 值：默认：3

  * 说明：每行的项目数；

### 事件处理程序

* ##### Navigated

  * 调用时机：用户点击项目跳转页面时；
  * 说明：可以在此事件里通过thisControl.Data获取点击Item的数据上下文;

### 属性、方法

* ##### ItemSource-获取/设置数据源（项目成员）；
* * 说明：数组；
  * 结构说明：Text：显示标题；Description：描述信息；ImageUrl：图片地址；ResourceUri：页面资源地址;Mode:展现方式，PC端设置为1，App端设置为0；ResourceText：显示页面标题；
* * 示例：
  * ```js
    //MetroNavView为控件对象
    MetroNavView.ItemSource = [{"Text":"项目1","ImageUrl":"图片地址1"," Description":"描述1","ResourceUri":"页面资源地址" ,"ResourceText":"页面标题","Mode":1},
        {"Text":"项目2","ImageUrl":"图片地址2"," Description":"描述2","ResourceUri":"页面资源地址" ,"ResourceText":"页面标题","Mode":1}];
    ```




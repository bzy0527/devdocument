# 加载UI LoadForm

作用：加载界面资源，显示界面；

### 设计属性

* ##### 活动标题

  * 类型：字符串；

  * 值：默认值：加载表单；

  * 说明：
* ##### 活动注释

  * 类型：字符串；

  * 值：

  * 说明：对活动的说明；
* ##### UI资源

  * 类型：字符串；

  * 说明：需要加载显示的功能组件的资源路径值；
* ##### UI标题

  * 类型：字符串；

  * 说明：展现的功能组件显示的导航栏标题；
* ##### 显示模式

  * 类型：数值；

  * 数值：示例：0；

  * 说明：0：视图控制器加载（整个页面覆盖，显示界面标题栏）；

    1：大尺寸设备停靠管理器加载模式（只限PC端使用）；

    2：弹出式窗口加载模式；

    3：整体页面切换模式（无返回按钮和功能组件标题）；

    4：大尺寸设备停靠管理器加载模式（只限PC端使用,会调用已加载界面的Load事件！！）；

    5：弹出窗口模式，会把弹出界面的控件居中显示（注：所有的控件需要布局到一个容器中，弹出窗口的背景色就是弹出界面所设置的背景色）；

    6：和模式0类似，不显示界面标题栏；

    7：表单替换（注：新加载的表单会完全替换现有表单进行显示）；

    注：不填写默认为0；其他数字则无效果，不会展示新的页面。
* ##### 上下文对象

  * 类型：

  * 说明：设置需要传递的上下文对象名或者值；

##### 回调函数参数：

* ##### uiview

  * 类型：加载页面的表单对象；

  * 说明：在加载表单的“调用成功”序列里可以直接获取；

##### 



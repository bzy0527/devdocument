# 文件上传 FileUploader

---

##### 作用：选择文件上传到服务器；

### 设计属性

* ##### 对象名称

  * 类型：字符串；

  * 值：

  * 说明：自定义控件对象名；
* ##### 上传地址

  * 类型：字符串；

  * 值：

  * 说明：文件上传的服务器地址；
* ##### 文件类型

  * 类型：字符串；

  * 值：

  * 说明：设置上传文件的类型；
* ##### 文件数量

  * 类型：数值；

  * 值：控制选择文件数量；
* ##### 最大文件限制

  * 类型：数值；

  * 值：

  * 说明：控制单个上传文件的最大限制，单位B；选择的文件超过限制大小将无法上传；

### 属性、方法

* ##### Files-属性，获取上传文件集合；

  * 说明：数组，每个元素都是一个文件对象；
* * 示例：
  * ```js
    [{"UploadFlag":1,"FileUrl":"",
    "name":"文件名","size":2032，,"type":"image/png
    "},{"UploadFlag":0,"FileUrl":"",
    "name":"文件名","size":2032，,"type":"image/png
    "}];
    //字段说明：UploadFlag-上传成功标识，1-上传成功，否则失败；
    //FileUrl-文件保存地址，上传成功时才会有文件地址；name-文件名称；size-文件大小，单位B；type-文件类型；
    ```

##### 




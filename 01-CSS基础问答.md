## 1、CSS是什么？

- CSS 指层叠样式表 (Cascading Style Sheets)
- CSS的作用是：可以给网页中的每一个元素设置样式（“化妆”、排版布局），让网页更加精美
- 样式通常存储在样式表中，⽬的也是为了解决内容与表现分离的问题
- 外部样式表(CSS⽂件)可以极⼤提⾼⼯作效率
- 多个样式定义可层叠为⼀，后者可以覆盖前者样式

## 2、 CSS 的语法结构？请给出样例代码

- 语法结构： 选择器 {属性:值; 属性:值; 属性:值; .... }

- 示例：

  ```css
  div {
  	display: inline-block;
  }
  ```

  

## 3、 CSS 的注释？ 

- 格式如下：

  ```css
  div {
  	/* display: inline-block; */
  }
  ```

  

## 4、HTML 中使用 CSS 的方式有哪几种？并描述一下他们的特点如何？

- CSS的使用方式有如下三种：

  - 内联样式（行内样式）

    - 就是在HTML的标签中使⽤style属性来设置css样式

    - 格式： <html标签 style="属性:值;属性:值;....">被修饰的内容</html标签>

    - 示例：

      ```html
      <p style="color:blue;font-size:20px;">在HTML中如何使⽤css内联样式</p>
      <!-- 特点：仅作⽤于本标签。-->
      ```

  - 内嵌样式

    - 就是在head标签中使⽤ <style> .... </style> 标签来设置css样式

    - 示例：

      ```html
      <style type="text/css">
      ....css样式代码
      </style>
      <!-- 特点：作⽤于当前整个⻚⾯ -->
      ```

  - 外部链入样式

    - 在head标签中使⽤标签导⼊⼀个css⽂件，在作⽤于本⻚⾯，实现css样式设置

    - 示例：

      ```html
      <link href="⽂件名.css" type="text/css" rel="stylesheet"/>
      ```

- 三种样式表特点总结

  | 样式表 |  优点 |  缺点  | 使⽤情况 |  控制范围 |
  | - | - | - | -| - |
  | ⾏内样式表  | 书写⽅便，权重⾼  |  没有实现样式和结构相分离  | 较少  | 控制⼀个标签（少）|
  | 内部样式表 | 部分结构和样式相分离  | 没有彻底分离 |  较多  | 控制⼀个⻚⾯（中） |
  | 外部样式表 | 完全实现结构和样式相分离  | 需要引⼊  | 最多，强烈推荐 | 控制整个站点（多） |

  
  












## 1. HTML 标签选择器如何使用？请给出样例代码 

- 使用方式

  就是把html标签作为选择符使⽤，如 p{....} ⽹⻚中所有p标签采⽤此样式

  如 p{....} ⽹⻚中所有p标签采⽤此样式

- 示例

  ```css
  p {
    background-color: #ddd;
  }
  ```

## 2. Class 类选择器如何定义和使用？请给出样例代码

- 定义： 

    .类名{样式....}  或 其他选择符名.类名{样式....}

- 使用方式

     在 <html标签 class="类名">...</html标签> 中使用，并且类选择符可以在⽹⻚中重复使⽤

- 示例

  ```css
  <style>
  .title {
    color: red;
    font-size:24px;
  }
  </style>
  ```

## 3. ID 选择器如何定义和使用？请给出样例代码 

- 定义：

  ​	\#id名{样式.....}

- 使用方式

     在 <html标签 class="类名">...</html标签> 中使用，id选择符只在⽹⻚中使⽤⼀次.

- 示例

  ```css
  #book {
    width: 200px;
  }
  ```

## 4. 请给出一段关联选择器样例代码 

- 示例

  ```css
  div p{color:red} /*只有div标签中的p标签才采⽤此样式(包括直接、间接子元素)*/
  div>span {font-size:18px;} /*只有div标签中的直接span标签采用此样式,不包括间接子元素*/
  ```

## 5.请给出一段组合选择器样例代码 

- 示例

  ```css
  h3,h4,h5{color:#ccc;} /*h3、h4和h5都采⽤此样式*/
  ```

## 6. CSS 中都有哪些关系选择器？请给出样例代码 

- 关系选择器：

  - div>p 选择所有作为div元素的⼦元素p
  - div+p 选择紧贴在div元素之后p元素
  - div~p 选择div元素后⾯的所有兄弟元素p

- 示例

  ```css
  div>p {
  	font-size: 20px; /*div元素的直接⼦元素p*/
  }
  div+p {
  	font-size: 22px; /*紧贴在div元素之后p元素*/
  }
  div>p {
  	font-size: 24px; /*div元素后⾯的所有兄弟元素p*/
  }
  ```

## 7. CSS 中都有哪些属性选择器？请给出样例代码 

- 属性选择器：

  - [attribute]选择具有attribute属性的元素。
  - [attribute=value]选择具有attribute属性且属性值等于value的元素。
  - [attribute~=value]选择具有attribute属性且属性值为⽤空以格分隔的字词列表，其中⼀个等于value的元素。
  - [attribute|=value]选择具有attribute属性且属性值为以val开头并⽤连接符"-"分隔的字符串的元素。
  - [attibute^=value]匹配具有attribute属性、且值以valule开头的E元素
  - [attribute$=value]匹配具有attribute属性、且值以value结尾的元素
  - [attribute*=value]匹配具有attribute属性、且值中含有value的元素

- 示例

  ```css
  /* 含有title属性的li标签采用此样式*/
  li[title]{color:red;}
  
  /*含有title属性值为bb的li标签采用此样式*/
  li[title="bb"]{color:red;}
  
  /*含有class属性值（以空格分隔开）中有aa的li标签采用此样式*/
  li[class~="aa"]{color:red;}
  
  /*含有class属性值（以-分隔开)以aa开头的li标签采用此样式*/
  li[class|="aa"]{color:red;}
  
  /*class属性值是以b子串开头的*/
  li[class^="b"]{font-size: 22px;}
  
  /*class属性值是以dd结尾的li标签*/
  li[class$="dd"]{font-size: 22px;}
  
  /*class属性值中含有bb的li标签*/
  li[class*="bb"]{font-size: 22px;}
  ```

## 

## 8. 请列出至少 6 个结构性伪类选择器，并对其说明功能 

- 结构性伪类选择器：

  - ::first-letter设置对象内的第⼀个字符的样式。
  - ::first-line设置对象内的第⼀⾏的样式。
  - :first-of-type匹配同类型中的第⼀个同级兄弟元素

  - :last-of-type匹配同类型中的最后⼀个同级兄弟元素
  - :first-child 匹配⽗元素的第⼀个⼦元素

  - :last-child 匹配⽗元素的最后⼀个⼦元素
  - :nth-child(n)匹配⽗元素的第n个⼦元素

## 9. 请列出至少 6 个状态性伪类选择器，并对其说明功能

- 状态性伪类选择器：
  - :link 设置超链接a在未被访问前的样式。
  - :visited 设置超链接a在其链接地址已被访问过时的样式
  - :active 设置元素在被⽤户激活（在⿏标点击与释放之间发⽣的事件）时的样式
  - :hover 设置元素在其⿏标悬停时的样式
  - :focus 设置元素在其获取焦点时的样式
  - :checked 匹配⽤户界⾯上处于选中状态的元素


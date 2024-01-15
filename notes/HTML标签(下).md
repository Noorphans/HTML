# HTML标签(下)

[toc]



## 表格标签

目标：能够写出表格

### 表格的主要作用

* 表格主要**用于显示、展示数据**，因为它可以让数据显示的非常的规整，可读性非常好。
* 特别是后台展示数据时，能够熟练运用表格就显得很重要。一个清爽简约的表格能够把繁杂的数据表现得很有条理。
* **表格**不是用来布局页面的,而是用来**展示数据**的，比如：

![表格1](http://images.newstar.net.cn/sally-imgs%E8%A1%A8%E6%A0%BC1.png) 





### 表格的基本语法

```html
<table>
 <tr>
 <td>单元格内的文字</td>
 ...
 </tr>
 ...
</table>
```

```html
 <!-- 三行三列 -->
  <table>
    <tr>
      <td>姓名</td>
      <td>性别</td>
      <td>年龄</td>
    </tr>
    <tr>
      <td>朱丽叶</td>
      <td>女</td>
      <td>45</td>
    </tr>
    <tr>
      <td>罗密欧</td>
      <td>男</td>
      <td>50</td>
    </tr>
  </table>
```

1. < table> </table> 是用于定义表格的标签。
2. `<tr> </tr>` 标签用于`定义表格中的行`，必须嵌套在 <table> </table>标签中。
3. `<td> </td>` 用于`定义表格中的单元格`，必须嵌套在<tr></tr>标签中。字母 **td 指表格数据**（table data），即**数据单元格的内容**。





### 表头单元格标签

* 一般表头单元格位于表格的**第一行或第一列**，**表头单元格**里面的**文本内容加粗**居中显示.
* <th> 标签表示 HTML 表格的表头部分(table head 的缩写)

```html
<table>
 <tr>
 <th>姓名</th>
 <th>性别</th>
 <th>电话</th>
 </tr>
 <tr>
  <td>小王</td>
  <td>女</td>
  <td>110</td>
 </tr>
 <tr>
  <td>小明</td>
  <td>男</td>
  <td>120</td>
 </tr>
</table>
```

![表头单元格标签](http://images.newstar.net.cn/sally-imgs%E8%A1%A8%E5%A4%B4%E5%8D%95%E5%85%83%E6%A0%BC%E6%A0%87%E7%AD%BE.png)





### 表格属性

表格标签这部分属性我们实际开发我们不常用，后面通过 CSS 来设置，目的有2个: 

1. 记住这些英语单词,后面 CSS 会使用.
2. 直观感受表格的外观形态.

![表格属性](http://images.newstar.net.cn/sally-imgs%E8%A1%A8%E6%A0%BC%E5%B1%9E%E6%80%A7.png) 

![image-20231227114311604](http://images.newstar.net.cn/sally-imgsimage-20231227114311604.png)





### 表格结构标签

* 使用场景:因为**表格**可能很长,为了更好的表示表格的语义，可以将表格**分割成 表格头部和表格主体**两大部分.
* 在表格标签中，分别用：`<thead>标签 表格的头部区域、<tbody>标签 表格的主体区域`. 这样可以更好的分清表格结构。
  1.  `<thead></thead>`：用于定义`表格的头部`。< thead> 内部必须拥有 < tr> 标签。 一般是位于第一行。
  2.  `<tbody></tbody>`：用于定义表格的主体，主要用于`放数据本体` 。
  3. 以上标签都是放在 < table>< /table> 标签中。

![image-20231228123615029](http://images.newstar.net.cn/sally-imgsimage-20231228123615029.png) 







### 合并单元格

特殊情况下,可以把多个单元格合并为一个单元格, 这里同学们会最简单的合并单元格即可

1. 合并单元格方式
2. 目标单元格 
5. 合并单元格的步骤

![合并单元格](http://images.newstar.net.cn/sally-imgs%E5%90%88%E5%B9%B6%E5%8D%95%E5%85%83%E6%A0%BC.png) 



#### 合并单元格方式

* 跨**行**合并：**rowspan**="合并单元格的个数" 
* 跨**列**合并：**colspan**="合并单元格的个数"



![image-20240115152633508](http://images.newstar.net.cn/sally-imgsimage-20240115152633508.png)  





#### 目标单元格：(写合并代码)

* 跨行：最上侧单元格为目标单元格, 写合并代码
* 跨列：最左侧单元格为目标单元格, 写合并代码

![image-20240115152829326](http://images.newstar.net.cn/sally-imgsimage-20240115152829326.png)  



#### 合并单元格三步曲

1. 先确定是跨行还是跨列合并。
2. 找到目标单元格. 写上合并方式 = 合并的单元格数量。比如：< td colspan="2"></td>。
3. 删除多余的单元格

![image-20231228154411351](http://images.newstar.net.cn/sally-imgsimage-20231228154411351.png)  







### 表格标签学习路线总结

表格学习整体可以分为三大部分:表格的相关标签、表格的相关属性、合并单元格



#### 表格的相关标签

table标签、tr行标签、td单元格标签、th表头标签、thead表格头部区域标签、tbody表格主体区域标签、

![image-20240115150343615](http://images.newstar.net.cn/sally-imgsimage-20240115150343615.png)  



#### 表格的相关属性

![表格属性](http://images.newstar.net.cn/sally-imgs%E8%A1%A8%E6%A0%BC%E5%B1%9E%E6%80%A7.png) 



#### 合并单元格

colspan、rowspan

![image-20231228155802996](http://images.newstar.net.cn/sally-imgsimage-20231228155802996.png) 









## 补充-定义表格标题标签

* `<caption>` 是HTML中用于定义表格标题的标签。
* 它必须位于`<table>` 元素内部，并且通常放置在**表格的开头**。
* `<caption>` 标签的内容将被显示为表格的标题，提供关于表格内容的简短描述或总结。
* 语法：

```html
<table>
  <caption>This is a Table Caption</caption>
   <!-- <caption><h2>This is a Table Caption</h2></caption> -->  
  <tr>
    <th>Header 1</th>
    <th>Header 2</th>
  </tr>
  <tr>
    <td>Row 1, Cell 1</td>
    <td>Row 1, Cell 2</td>
  </tr>
  <tr>
    <td>Row 2, Cell 1</td>
    <td>Row 2, Cell 2</td>
  </tr>
</table>
```

结论： `<caption>` 直接包含文本内容，这样就定义表格的标题。也可以嵌套标题标签，自定义设置不同等级标题







## 列表标签

目标：能够写出无序列表

* 表格是用来显示数据的，那么**列表就是用来布局的**。
* **列表**最大的特点就是整齐、整洁、有序，它作为布局会更加自由和方便。
* 根据使用情景不同，列表可以分为三大类：**无序列表**、**有序列表**和**自定义列表**。 

 







### 无序列表（重点）

* **< ul>** 标签表示 HTML 页面中项目的无序列表，一般会以项目符号呈现列表项，而列表项使用 **< li>** 标签定义。
* 无序列表的基本语法格式如下：

```html
 <ul>
    <li>纯全芝士棒</li>
    <li>榴莲披萨</li>
    <li>酸奶水果披萨</li>
    <li>酥小满牛肉饼</li>
    <li>酱香饼</li>
    <li>葱油饼</li>
    <li>梅干菜饼</li>
    <li>烤羊排</li>
    <li>炸鸡排</li>
    <li>炸猪排</li>
    <li>烤面筋</li>
    <li>烤五花肉</li>
    <li>烤火腿</li>
    ...
  </ul>
```

结论：

1. 无序列表的各个列表项之间没有顺序级别之分，是并列的
2. **< ul>< /ul> 中只能嵌套 < li>< /li>**，直接在 < ul>< /ul> 标签中输入其他标签或者文字的做法是不被允许的
3. **< li> 与 < /li> 之间相当于一个容器，可以容纳所有元素。**
4. 无序列表会带有自己的样式属性，但在实际使用时，我们会使用 CSS 来设置

![image-20240104095829074](http://images.newstar.net.cn/sally-imgsimage-20240104095829074.png)







### 有序列表（理解）

* 有序列表即为有排列顺序的列表，其各个列表项会按照一定的顺序排列定义。
* 在 HTML 标签中，< ol> 标签用于定义有序列表，列表排序以数字来显示，并且使用 <li> 标签来定义列表项。
* 有序列表的基本语法格式如下：

```html
 <ol>
    <li>纯全芝士棒</li>
    <li>榴莲披萨</li>
    <li>酸奶水果披萨</li>
    <li>酥小满牛肉饼</li>
    <li>酱香饼</li>
    <li>葱油饼</li>
    <li>梅干菜饼</li>
    ...
  </ol>
```

结论：

1. < ol>< /ol>中只能嵌套< li>< /li>，直接在< ol>< /ol>标签中输入其他标签或者文字的做法是不被允许的。

2. < li> 与 < /li>之间相当于一个容器，可以容纳所有元素。

3. 有序列表会带有自己样式属性，但在实际使用时，我们会使用 CSS 来设置。

![image-20240104095220514](http://images.newstar.net.cn/sally-imgsimage-20240104095220514.png)









###  自定义列表（重点）

* 自定义列表的使用场景:自定义列表常用于对术语或名词进行解释和描述，定义列表的列表项前没有任何项目符号。

* 在HTML标签中，**< dl>** 标签用于定义描述列表（或定义列表），该标签会与 **< dt>**（定义项目/名字）和**< dd>**（描述每一个项目/名字）一起使用。

* 其基本语法如下：

```html
<dl>
 <dt>名词1</dt>
 <dd>名词1解释1</dd>
 <dd>名词1解释2</dd>
</dl>
```

结论:

1. **< dl>< /dl> 里面只能包含 < dt> 和 < dd>**。
2. < dt> 和 <dd>个数没有限制，经常是一个<dt> 对应多个<dd>。



\- 举例说明：

```html
 <dl>
    <dt>帮助中心</dt>
    <dd>账户管理</dd>
    <dd>购物指南</dd>
    <dd>订单操作</dd>
  </dl>
```

![image-20240115152020196](http://images.newstar.net.cn/sally-imgsimage-20240115152020196.png)





### 列表总结

![image-20240115150441877](http://images.newstar.net.cn/sally-imgsimage-20240115150441877.png) 

> **注意：**
>
> 1. 掌握何时用无序列表， 何时用自定义列表。
>
>    * 若遇到排列整齐，每一个都很简单且没有相关顺序就用无序列表ul
>
>    * 若遇到上面有个小标题，下面是围绕小标题来说明的就用自定义列表dl
>
> 2. 无序列表和自定义列表代码怎么写？
>    * 无序列表先有一个父亲ul，里面再包含多个小li
>    * 自定义列表先有一个父亲dl，里面包含dt和dd且**一个dt对应多个dd**
>
> 3. 列表布局在学习完 CSS 后再来完成。









## 表单标签

* 目标：能够写出3~4个常用input表单类型、下拉列表表单、使用表单元素实现注册页面，独立查阅W3C文档

* 现实中的表单，我们去银行办理信用卡填写的单子：

![image-20240104103108137](http://images.newstar.net.cn/sally-imgsimage-20240104103108137.png) 



* 网页中的表单展示：

![image-20240115150506082](http://images.newstar.net.cn/sally-imgsimage-20240115150506082.png) 





1. **为什么需要表单**

使用表单目的是为了**收集用户信息**。在我们网页中， 我们也需要跟用户进行交互，收集用户资料，此时就需要表单



2. **表单的组成**

在 HTML 中，一个完整的表单通常由**表单域、表单控件（也称为表单元素）**和 **提示信息**3个部分构成。

![image-20240115150613673](http://images.newstar.net.cn/sally-imgsimage-20240115150613673.png) 







### 表单域

*  **表单域**是一个**包含表单元素的区域**。目的是把元素信息送给服务器(后台)

* 在HTML标签中， **< form>** 标签用于定义表单域，以实现用户信息的收集和传递。**它会把它范围内的表单元素信息提交给服务器**

```html
<form action=“url地址” method=“提交方式” name=“表单域名称">
    各种表单元素控件
</form>
```

\- 举例说明：

```html
<!-- 假设把表单元素提交给demo.php进行处理,提交方式post，表单域名称name1 -->
  <form action="demo.php" method="post" name="name1">

  </form>
```



* 常用属性：

![image-20240104103645855](http://images.newstar.net.cn/sally-imgsimage-20240104103645855.png) 

>* 在这里暂时不用表单域提交数据,只需要写上 form 标签即可. 等学习服务器编程阶段再使用.
>
>* 这里只需要记住两点:
>  1. 在我们写表单元素之前,应该有个表单域把他们进行包含.
>  2. **表单域是 form标签**









### 表单控件(表单元素)-重点

* 表单控件也叫表单元素。在表单域中可以定义各种表单元素，这些表单元素就是允许用户在表单中输入或者选择的内容控件。
* 如**input输入表单元素**、**select下拉表单元素**、**textarea 文本域元素**





#### input输入表单元素

* 在英文单词中，input 是输入的意思，而在表单元素中 **< input> 标签用于收集用户信息**。
* 在 < input> 标签中，包含一个**type**属性，根据不同的**type**属性值，输入字段拥有很多种形式（可以是文本字段、复选框、掩码后的文本控件、单选按钮、按钮等）。

```html
<input type="属性值" />
```

> **注：**
>
> 1. < input /> 标签为**单标签**
> 2. type 属性设置不同的属性值用来指定不同的控件类型

```html
<form>
    <!-- text 文本框 用户可以里面输入任何文字 -->
    用户名：<input type="text">
</form>
```





##### type属性

![image-20240115150653328](http://images.newstar.net.cn/sally-imgsimage-20240115150653328.png) 



\- 举例说明：

```html
 <form>
     <!-- text 文本框 用户可以里面输入任何文字 -->
    用户名：<input type="text">
     
    <!-- password 密码框 用户看不见输入的密码 -->
    密&nbsp;&nbsp;&nbsp;码：<input type="password"> <br>

    <!-- radio 单选按钮 实现多选一 -->
    性&nbsp;&nbsp;&nbsp;别：男<input type="radio"> 女<input type="radio"><br>
     
    <!-- checkbox 复选框 实现多选 -->
    爱&nbsp;&nbsp;&nbsp;好：吃美食<input type="checkbox"> 旅游<input type="checkbox"> 睡觉<input type="checkbox"><br>
     
     <!-- 点击了提交按钮,可以把 表单域 form 里面的表单元素 里面的值 提交给后台服务器 -->
     <!-- 或者点击提交按钮时，表单中的数据将会被发送到 `action` 属性指定的 URL 上。 -->
    <input type="submit" value="免费注册">
     
     <!-- 重置按钮可以还原表单元素初始的默认状态 -->
    <input type="reset" value="重新填写"><br>
     
     <!-- 普通按钮 button，不提交数据而是执行某件事 后期结合js 搭配使用-->
    <input type="button" value="获取短信验证">
     
     <!-- 文件域 使用场景 上传文件使用的 -->
    上传头像: <input type="file">
     
     <!-- 隐藏域：网页上看不到，但是表单提交的时候数据会自动提交给服务器 -->
     <input type="hidden" > 
  </form>
```







##### 其他常用属性

![image-20240115150745980](http://images.newstar.net.cn/sally-imgsimage-20240115150745980.png) 

**解析**：

1. name 和value 是每个表单元素都有的属性值,主要给后台人员使用

2. **checked属性主要针对于单选按钮和复选框**, 主要作用一打开页面,就要可以默认选中某个表单元素.

3. maxlength 是用户可以在表单元素输入的最大字符数, 一般较少使用.

   ```html
   <form>
      用户名：<input type="text" name="username" value="请输入用户名" maxlength="6"> 
   </form>
   ```

   



###### name属性(重点)

* name属性：当前input表单元素的名字，后台可以通过这个name属性找到这个表单，`name`的主要作用就是用于`区别不同表单`

* 要求**单选按钮和复选框要有相同的name值** 即`单选框和复选框name必须一致`，value可以不一样

* 为什么单选框和复选框name值要相同？

  * 通过给单选框和复选框起相同的名字，系统就能理解哪些选项是互斥的（只能选一个），哪些是可以同时选择的。以便更有效地处理用户提交的表单数据。

  * radio (或者checkbox）如果是一组，我们必须给他们命名相同的名字 

    

  \- 通俗理解：

  1. 单选框（radio buttons）就像是你在“比萨大小”这个选项上做选择，比如“小号”、“中号”、“大号”等。而这些单选框都有一个相同的名字，比如说叫做“pizza_size”。这样，系统就知道你只能选一个尺寸，不能同时选两个或三个。
  2. 复选框（checkboxes）就像是你在“配料”这个选项上做选择，比如“芝士”、“火腿”、“蘑菇”等。同样，所有的复选框也有相同的名字，比如“toppings”。这样，系统就知道你可以选择多个配料，因为它们属于同一个组



\- 举例说明：

```html
 <form>
    <!-- radio 单选按钮 实现多选一 -->
    <!-- name 是表单元素名字 这里性别单选按钮必须有相同的名字name 才可以实现多选1 -->
    性&nbsp;&nbsp;&nbsp;别：男<input type="radio" name="sex"> 女<input type="radio" name="sex"><br>
    <!-- checkbox 复选框 实现多选 -->
    爱&nbsp;&nbsp;&nbsp;好：吃美食<input type="checkbox" name="hobby"> 旅游<input type="checkbox" name="hobby"> 睡觉<input
      type="checkbox" name="hobby">
  </form>
```





###### value属性

* 可以给这些表单元素设置 value 属性=“值”，有些表单元素想刚打开页面就默认显示几个文字。

  ```html
  用户名: <input type="text" value="请输入用户名" />
  ```

* value值只在文本框显示效果，单选和复选框在页面中看不到效果，而是针对后台使用，更关注数据的提交，而不是页面的直观显示

* 对于安全性原因，密码字段通常不建议设置默认值（使用`value`属性）。

  * 如果密码字段中设置了默认值，用户可能会不小心或者出于方便的目的忽略更改密码，从而增加安全风险。
  * 如果确实需要在页面中显示一些默认值或者提示，可以考虑使用占位符（placeholder）属性，而不是直接设置`value`。占位符是一种在用户未输入任何内容时在输入字段中显示的灰色文本，用户一旦开始输入，占位符就会消失。





###### checked属性

- 单选按钮和复选框可以设置checked 属性, **checked="checked"**,当页面打开时候就可以默认选中这个按钮,表示**默认选中状态**
- **单选框只能给其中一个加checked，复选框可以多加**

```html
<form>
<!-- 单选按钮和复选框可以设置checked 属性, 当页面打开的时候就可以默认选中这个按钮 -->
性别：男<input type="radio" name="sex" value="男"> 女<input type="radio" name="sex" value="女" checked="checked"><br>
<!-- checkbox 复选框 实现多选 -->
爱好：吃美食<input type="checkbox" name="hobby" checked="checked"> 旅游<input type="checkbox" name="hobby" checked="checked"> 睡觉<input type="checkbox" name="hobby">
</form>
```

![image-20240105160107644](http://images.newstar.net.cn/sally-imgsimage-20240105160107644.png) 



##### label标签

* **< label>** 标签为 input 元素定义标注（标签）。

* **< label>** 标签用于绑定一个表单元素, 当点击< label> 标签内的文本时，浏览器就会自动将焦点(光标)转到或者选择对应的表单元素上,用来增加用户体验.

* 语法：

  ![image-20240115151905885](http://images.newstar.net.cn/sally-imgsimage-20240115151905885.png)

  解析：`label`标签通过`for`属性与输入框关联，而输入框的`id`属性值为"sex"。这两者的匹配关系建立了联系。当用户点击"用户名："这个标签时，浏览器会自动将焦点聚焦在id为"sex"的输入框上，使用户可以直接开始输入。

  

  > **核心**：label标签的`for属性`应当与相关元素的`id属性相同`。通过确保`for`与`id`匹配，可以使用户更容易地导航和理解表单。









#### select下拉表单元素

* 在页面中，如果有多个选项让用户选择，并且想要节约页面空间时，我们可以使用**< select>**标签控件定义**下拉列表**。

  ![image-20240115151725237](http://images.newstar.net.cn/sally-imgsimage-20240115151725237.png) 

* 语法：

```html
  <select>
    <option>选项1</option>
    <option>选项2</option>
    <option>选项3</option>
      ...
  </select>
```

> **注**：
>
> 1. < select> 中**至少包含一对< option>** 。
>
> 2. 在**< option> 中**定义 **selected =“ selected "** 时，当前项即为**默认选中项**。



\- 举例说明：

```html
 <form>
    籍贯：
    <select>
      <option>山东</option>
      <option>北京</option>
      <option>天津</option>
      <option selected="selected">南京</option>
    </select>
  </form>
```







#### textarea文本域元素

* 当用户**输入内容较多**的情况下，我们就不能使用文本框表单了，此时可以**使用 < textarea> 标签**。
* 在表单元素中，`< textarea>` 标签是用于`定义多行文本输入`的控件。
* 使用多行文本输入控件，可以输入更多的文字，该控件常见于留言板，评论
* 语法：

```html
<textarea rows="3" cols="20">
 文本内容
</textarea>
```

> **注**：
>
> 1. 通过 < textarea> 标签可以轻松地创建多行文本输入框。
>
> 2. cols=“每行中的字符数” ，rows=“显示的行数”，**我们在实际开发中不会使用，都是用 CSS 来改变大小**。



\- 举例说明：

```html
  <form>
    今日反馈：
    <textarea cols="50" rows="20">
      这个反馈留言是textarea来做的. 
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Ullam nam soluta laboriosam veritatis! Praesentium perferendis consectetur, vel id harum distinctio ipsum, voluptas odio sapiente quidem repellat temporibus nulla porro quod!
      Lorem ipsum, dolor sit amet consectetur adipisicing elit. Cupiditate, nostrum velit! Quae, exercitationem pariatur molestias ducimus voluptatum iusto cum dignissimos. Officiis repellat numquam, recusandae placeat dolorum fugit obcaecati ipsa ea?
      Lorem ipsum dolor, sit amet consectetur adipisicing elit. Libero deleniti labore incidunt eum facilis reiciendis laboriosam eius animi obcaecati eos placeat, vel quo velit culpa. Porro non voluptates voluptatibus dignissimos!
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Consectetur molestiae excepturi repellendus veniam accusantium, hic dignissimos eos cum vero aliquid quaerat. Vitae error iure sapiente! Hic dicta corporis sunt temporibus?
    </textarea>
  </form>
```









### 表单元素总结

> **注**：input输入表单元素、select下拉表单元素、textarea文本域表单元素.这三组都应包含在form表单域里面,并且name属性.

![image-20240115151510027](http://images.newstar.net.cn/sally-imgsimage-20240115151510027.png) 

* 有三个名字非常相似的标签：
  1. 表单域 form : 提交区域内表单元素给后台服务器
  2. 文件域 file ：是input type 属性值 : 上传文件
  3. 文本域 textarea : 可以输入多行文字, 比如留言板 网站介绍等…

* 当前阶段不需要提交表单元素,所以只负责表单元素的外观形态即可.





## 学会查阅文档

推荐的网址：

* 百度: http://www.baidu.com
* W3C : http://www.w3school.com.cn/
* MDN: https://developer.mozilla.org/zh-CN/
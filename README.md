# form表单作用及常用input标签
表单在网页中主要负责数据采集功能。表单也是用来提交资料、意见，规范流程执行过程的格式。

## 常用input标签：

a. 文本框：是一种让访问者直接输入内容的表单对象，通常被用来填写比较简短的回答，如姓名、地址等。
代码：
```
<input type="text "name="xx" size="xx" maxlength="xx "value="xx">
属性：type="text"定义单行文本输入框；
name属性定义文本框的名称，要保证数据的准确采集，必须定义一个独一无二的名称；
size属性定义文本框的宽度，单位是单个字符宽度；
maxlength属性定义最多输入的字符数;
value属性定义文本框的初始值。
```
b. 多行文本框：也是一种让访问者自己输入内容的表单对象，但能让访问者填写较长的内容。
代码：
```
<textarea name="xx" cols="xx" wrap="virtual"></textarea>
属性：name属性定义多行文本框的名称，要保证数据的准确采集，必须定义一个独一无二的名称；
cols属性定义多行文本框的宽度，单位是单个字符宽度；
rows属性定义多行文本框的高度，单位是单个字符宽度；
wrap属性定义输入内容大于文本域时显示的方式，可选值如下：默认值是文本自动换行；当输入内容超过文本域的右边界时会自动转到下一行，而数据在被提交处理时自动换行的地方不会有换行符出现； Off，用来避免文本换行，当输入的内容超过文本域右边界时，文本将向左滚动，必须用Return才能将插入点移到下一行；
 Virtual，允许文本自动换行；
 Physical，让文本换行，当数据被提交处理时换行符也将被一起提交处理。
```
c.密码框：是一种特殊的文本域，用于输入密码。当访问者输入文字时，文字会被星号或其它符号代替，而输入的文字会被隐藏。
代码：
```
<input type="password" name="xx" size="xx" maxlength="xx">
属性：type="password"定义密码框；
name属性定义密码框的名称，要保证数据的准确采集，必须定义一个独一无二的名称；
size属性定义密码框的宽度，单位是单个字符宽度；
maxlength属性定义最多输入的字符数。
```
d. 隐藏域：用来收集或发送信息的不可见元素，对于网页的访问者来说，隐藏域是看不见的。当表单被提交时，隐藏域就会将信息用你设置时定义的名称和值发送到服务器上。
代码：
```
<input type="hidden" name="xx" value="xx">
属性：
type="hidden"定义隐藏域；
name属性定义隐藏域的名称，要保证数据的准确采集，必须定义一个独一无二的名称；
value属性定义隐藏域的值。
```
e. 复选框：允许在待选项中选中一项以上的选项。每个复选框都是一个独立的元素，都必须有一个唯一的名称。
代码：
```
<input type="checkbox" name="xx" value="xx">
属性：
type="checkbox"定义复选框；
name属性定义复选框的名称，要保证数据的准确采集，必须定义一个独一无二的名称；
value属性定义复选框的值。
```
f. 单选框：当需要访问者在待选项中选择唯一的答案时，就需要用到单选框了。
代码：
```
<input type="radio" name="xx" value="xx">
属性：
type="radio"定义单选框；
name属性定义单选框的名称，要保证数据的准确采集，单选框都是以组为单位使用的，在同一组中的单选项都必须用同一个名称；
value属性定义单选框的值，在同一组中，它们的域值必须是不同的。
```
g. 文件上传框：有时候，需要用户上传自己的文件，文件上传框看上去和其它文本域差不多，只是它还包含了一个浏览按钮。访问者可以通过输入需要上传的文件的路径或者点击浏览按钮选择需要上传的文件。
注意：在使用文件域以前，请先确定你的服务器是否允许匿名上传文件。表单标签中必须设置ENCTYPE="multipart/form-data"来确保文件被正确编码；另外，表单的传送方式必须设置成POST。
代码：
```
<input type="file" name="xx" size="xx" maxlength="xx">
属性：
type="file"定义文件上传框；
name属性定义文件上传框的名称，要保证数据的准确采集，必须定义一个独一无二的名称；
size属性定义文件上传框的宽度，单位是单个字符宽度；
maxlength属性定义最多输入的字符数。
```
h.下拉选择框：下拉选择框允许你在一个有限的空间设置多种选项。
代码：
```
<select name="xx" size="xx" multiple> 
   <option value="xx"selected>
   </option>
</select>
属性：
size属性定义下拉选择框的行数；
name属性定义下拉选择框的名称；
multiple属性表示可以多选，如果不设置本属性，那么只能单选；
value属性定义选择项的值；
selected属性表示默认已经选择本选项。
```
i. 提交按钮：提交按钮用来将输入的信息提交到服务器。
代码：
```
<input type="submit" name="xx" value="xx">
属性：
type="submit"定义提交按钮；
name属性定义提交按钮的名称；
value属性定义按钮的显示文字。
```
j. 复位按钮：用来重置表单。
代码：
```
<input type="reset" name="xx" value="xx">
属性：
type="reset"定义复位按钮；
name属性定义复位按钮的名称；
value属性定义按钮的显示文字。
```
k. 一般按钮：用来控制其他定义了处理脚本的处理工作。
代码：
```
<input type="button" name="xx" value="xx" onClick="xx">
属性：
type="button"定义一般按钮；
name属性定义一般按钮的名称；
value属性定义按钮的显示文字；
onClick属性，也可以是其它的事件，通过指定脚本函数来定义按钮的行为。
```
# post与get
## GET方式：
1、GET方式是以实体的方式得到由请求URL所指定资源的信息，如果请求URL只是一个数据产生过程，那么最终要在响应实体中返回的是处理过程的结果所指向的资源，而不是处理过程的描述。也就是说，GET的到的信息是资源，而不是资源的处理过程。
2、请的求的数据会附加在URL之后，以？分隔URL和传输数据，多个参数用&连接。URL编码格式采用的是ASCII编码，而不是Unicode，即所有的非ASCII字符都要编码之后再传输。
3、因为URL的长度限制，GET方式传输的数据大小有所限制，传送的数据量不超过2KB。
4、GET方式服务器端用Request.QueryString获取变量的值。
5、GET方式传输的参数安全性低，因为传输的数据会显示在请求的URL中。
##W POST方式：
1、用来向目的服务器发出请求，要求它接收被附在请求后的实体，并把它当做请求队列中请求URL所指定资源的附加新子项。
2、POST方式将表单内各个字段和内容放置在HTML HEADER中一起传送到Action属性所指定的URL地址，用户是看不到这个过程的。
3、POST方式传送的数据量比较大，一般被默认为没有限制，但是根据IIS的配置，传输量也是不同的。
4、POST方式在服务器端用Request.Form获取提交的数据。
5、POST方式传输的数据安全性较高，因为数据传输不是明显显示的。
总结：POST和GET方式的安全性是相对的，另外也要看是从哪个角度来看的。从数据传输过程方面来看，POST方式是更加安全的，但是从对服务器数据的操作来看，POST方式的安全性又是比较低的。即使是传输过程用POST来执行，安全性也是相对的，如果了解HTTP协议漏洞，通过拦截发送的数据包，同样可以修改交互数据，所以这里的安全不是绝对的。
# input中name的作用
用途1: 作为可与服务器交互数据的HTML元素的服务器端的标示，比如input、select、textarea、和button等。我们可以在服务器端根据其Name通过Request.Params取得元素提交的值。
用途2: HTML元素Input type='radio'分组，我们知道radio button控件在同一个分组类，check操作是mutex的，同一时间只能选中一个radio，这个分组就是根据相同的Name属性来实现的。
用途3: 建立页面中的锚点，我们知道link是获得一个页面超级链接，如果不用href属性，而改用Name，如：，我们就获得了一个页面锚点。
用途4: 作为对象的Identity，如Applet、Object、Embed等元素。比如在Applet对象实例中，我们将使用其Name来引用该对象。
用途5: 在IMG元素和MAP元素之间关联的时候，如果要定义IMG的热点区域，需要使用其属性usemap，使usemap="#name"(被关联的MAP元素的Name)。
用途6: 某些特定元素的属性，如attribute，meta和param。例如为Object定义参数或Meta中。
# placeholder 属性
占位符
```
![](http://upload-images.jianshu.io/upload_images/7279690-bc0dd4047eb834c4.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](http://upload-images.jianshu.io/upload_images/7279690-9afa06e8df80c53a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
```
# type=hidden隐藏域
隐藏域在页面中对于用户是不可见的，在表单中插入隐藏域的目的在于收集或发送信息，以利于被处理表单的程序所使用
（隐藏只是在网页页面上面不显示输入框，但是虽然隐藏了，还是具有form传值功能。
一般用来传值，而不必让用户看到。
作用：
1 隐藏域在页面中对于用户是不可见的，在表单中插入隐藏域的目的在于收集或发送信息，以利于被处理表单的程序所使用。浏览者单击发送按钮发送表单的时候，隐藏域的信息也被一起发送到服务器。
2 有些时候我们要给用户一信息，让他在提交表单时提交上来以确定用户身份，如sessionkey，等等．当然这些东西也能用cookie实现，但使用隐藏域就简单的多了．而且不会有浏览器不支持，用户禁用cookie的烦恼。
3 有些时候一个form里有多个提交按钮，怎样使程序能够分清楚到底用户是按那一个按钮提交上来的呢？我们就可以写一个隐藏域，然后在每一个按钮处加上
```
onclick="document.form.command.value="xx""
```
然后我们接到数据后先检查command的值就会知道用户是按的那个按钮提交上来的。
4 有时候一个网页中有多个form，我们知道多个form是不能同时提交的，但有时这些form确实相互作用，我们就可以在form中添加隐藏域来使它们联系起来。
5js不支持全局变量，但有时我们必须用全局变量，我们就可以把值先存在隐藏域里，它的值就不会丢失了。
6 还有个例子，比如按一个按钮弹出四个小窗口，当点击其中的一个小窗口时其他三个自动关闭．可是IE不支持小窗口相互调用，所以只有在父窗口写个隐藏域，当小窗口看到那个隐藏域的值是close时就自己关掉。

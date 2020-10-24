## html重难点

### 工具

    http-serve
    yarn global add http-server
    使用 http-serve -c-1

    或者
    yarn global add parcel
    使用 parcel xxx.html

### a标签
  
* 属性
  
  * href 超链接
  ```html
      <a href="//google.com" download>超链接</a>

      <a href="./index.html">c.html</a>

      <a href="javascript:alert(1);">JavaScript伪协议</a>

      一般<a href="javascript:;"></a>什么都不做的a标签

      <a href="xxx"></a> xxx为id,跳转到指定id

      <a href="mailto:xxxx@xxxmail.com">发邮件</a>

      <a href="tef:13845678912">打电话</a>手机上会自动呼起拨号键
    ```
  * target 指定在哪个窗口打开超链接 一般使用 `_blank`
  
      内置名字：

      _blank 

      _top

      _parent

      _self

  * download 一般不使用
  * rel=noopener 暂时不用了解
* 作用
  * 跳转外部页面
  * 跳转内部锚点
  * 跳转到邮箱或电话等

### table标签

table标签里有三个标签
    <table>
        <thead>
            <tr> 行row
                <th></th>表头
            </tr>
        </thead>
        <tbody>
            <tr> 行row
                <td></td>
            </tr>
        </body>
        <tfoot>
            <tr> 行row
                <td>空</td>
            </tr>
        </tfoot>
    </table>

相关样式

    table-layout
    border-collapse border和border之间是否合并
    border-spacing  控制border之间的间距


### img标签

    <img src="">

* 作用
  
    发出get请求，展示一张图片

* 属性
  
    alt/height/width/src

* 事件
  
    onload/onerro  加载成功onload,加载失败noerrro

```js
    html
    <img src="" id="xxx">

    js
    xxx.onload = function(){
        console.log("图片加载失败")
    }
    xxx.onerror = function(){
        console.log("图片加载失败")
    }
```
* 响应式

     max-width:100%

* 可替换元素

### form标签

* 作用

发get或post请求，然后刷新页面

* 属性

action/autocomplete/method/target
autocomplete 自动填充

* 事件

onsubmit

```html
<form action="/xxx" method="POST" autocomplete="on">
    <input name="username" type="text">
    <input type="submit">
</form>
```

### input标签

* 作用

让用户输入内容

* 属性
    * 类型type
    button/checkbox/email/file/hidden/number/password/radio/search/submit/tel/text
    * 其他
    name/autofocus/checked/disabled/maxlength/pattern/value/placeholder

* 事件
    onchange/onfocus/onblur

* 验证器
    require
    HTML5新增功能

### 其他输入标签

* 标签
  * select+option
  * textarea
  * label
* 注意事项
  * 一般不监听input的click事件
  * form里面的input要有name
  * form里要放一个type=submit才能触发submit事件

### 其他标签

* 标签
  * video
  * audio
  * canvas
  * svg(矢量)
* 注意事项
  * 这些标签的兼容性一定要查看文档

### 书推荐

《网道HTML教程》

### 看书技巧

三上：马上 枕上 厕上

### 工具

代码链接

jsbin

饥人谷jsbin

[代码沙盒](codesandbox.io)

head和body一般不缩进

### 章节标签
* h1~h6
* section 章节
* article 文章
* p
* header 头部
* footer 脚部
* main 主要内容
* aside 旁支内容
* div 划分


### 全局属性
所有标签都有的属性
* class
* contenteditable (元素可以被编辑)
* hidden （让标签看不见）  
    <header hidden>顶部</header>
* id   不到万不得已不要用id,id不能是windows里的全局属性
* style
* tabindex 响应tab键,-1代表tab不访问，0代表最后访问
    <header tabindex=1></header>
* title 鼠标浮上这个元素，会显示title的内容

### 默认样式
 [reset.css](https://gist.github.com/FrankFang/df5e57a0799823ed89a960a642b3a1e2)

### 经常使用的内容标签

* ol 有序列表
  ```html
  <ol>
    <li></li>
    <li></li>
  </ol>
  ```
* ul 无序列表
  
  ```html
  <ul>
    <li></li>
    <li></li>
  </ul>
  ```

* dl+dt+dd 之定义列表
  
  ```html
  <dl>
    <dt>11</dt>
    <dd>22</dd>
  </dl>
  ```
* pre 保留空格，tab，回车，这样连续空格就不会压缩成一个

```html
<pre>
第一章：        工作内容
</pre>
```

* code (可以使用pre保留空格), 可以用来包裹代码片段
* em 语气上的强调
* strong 内容本身的重要性
* quote 行内
* blockquote 块级
# 第二章 HTML中使用JS
## 1. <scipt>元素
  使用<script>向HTML中插入JS
  其属性有async,charset,defer,language,src,type共6种
### 1.1 使用方式
#### 1.1.1 直接嵌入（为script指定type属性）
  <scipt type="text/javascript">
    function sayHi() {
      alert("Hi");
    }
  </script>
  解释器对<script>中的所有代码求值完毕之前，页面中的其他内容不会被浏览器加载或显示

#### 1.1.2 外部文件
  给script指定src属性。但是一旦使用了src，那么<script>和</script>标签之间不能再包含额外的js代码，是不会被解析的。
### 1.2 标签位置
  为了避免渲染阻塞，将标签一般放在<body>元素中页面内容的后面
  <body>
    页面内容
    <script>...</script>
  </body>
### 1.3 延迟脚本
  给脚本添加der

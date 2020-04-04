# css兼容性有哪几种处理方案

 1. 浏览器CSS样式初始化
 2. 浏览器私有属性
 3. CSS hack
 4. 自动化插件 Autoprefixer
 
 ## 浏览器CSS样式初始化
 1. 传统的css reset：去除所有的浏览器的默认样式,
 2. Normalize.css：与许多CSS重置不同，保留有用的默认值。标准化各种元素的样式。更正错误和常见的浏览器不一致问题。通过细微的修改来提高可用性。使用详细注释说明代码的作用。github地址： <a href='https://github.com/necolas/normalize.css'>Normalize.css</a>


  ## 浏览器私有属性
 
 1. 对于私有属性的顺序要注意，把标准写法放到最后，兼容性写法放到前面
 2. 常用的前缀有：
- -moz代表firefox浏览器私有属性
- -ms代表IE浏览器私有属性
- -webkit代表chrome、safari私有属性
- -o代表opera私有属性


## CSS hack
针对不同浏览器或者不同版本写特定的样式，CSS hack的写法大致归纳为3种：条件hack、属性级hack、选择符级hack。

 4. 自动化插件 Autoprefixer
 把css样式的兼容性交给了打包工具
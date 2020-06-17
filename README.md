CodeBeautify 
### 介绍

基于prismjs的代码语法高亮typecho插件，支持众多常见的代码语言高亮显示，提供11种代码高亮风格自由切换，支持显示代码语言类型、行号，以及支持复制代码到剪切板功能

### 激活

以Handsome主题为例：

第 1 步：下载本插件，解压，放到 usr/plugins/ 目录中；

第 2 步：文件夹名改为 CodeBeautify

第 3 步：登录管理后台，激活插件 （请勿与其它同类插件同时启用，以免互相影响）

第 4 步：设置：选择主题风格，是否显示行号等。

### Pjax

如果你的网站有开启Pjax

请把以下代码添加到回调函数的地方，在你使用的主题设置里看看

```javascript
if (typeof Prism !== 'undefined') {
var pres = document.getElementsByTagName('pre');
                for (var i = 0; i < pres.length; i++){
                    if (pres[i].getElementsByTagName('code').length > 0)
                        pres[i].className  = 'line-numbers';}
Prism.highlightAll(true,null);}
```

### prism.js:
```
https://prismjs.com/download.html#themes=prism-coy&languages=markup+css+clike+javascript+aspnet+bash+c+csharp+cpp+css-extras+dart+docker+git+go+groovy+java+json+kotlin+less+markdown+markup-templating+nginx+objectivec+php+plsql+powershell+properties+python+jsx+tsx+solidity+sql+swift+typescript+yaml&plugins=line-numbers+highlight-keywords+inline-color
```

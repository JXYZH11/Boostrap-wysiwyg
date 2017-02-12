# Boostrap-wysiwyg
Boostrap富文本编辑器

1、引入文件

css：
①bootstrap-combined.no-icons.min.css
②bootstrap-responsive.min.css
③font-awesome.css

重点来了，font-awesome要去官网下载3.0.2的版本才能使用，最新的版本不行，其他的版本不行，font文件夹也要用3.0.2的，不然会报错，找不到文件，编辑器的图片出不来。

js：
①jQuery.min.js（JQuery支持）
②jquery.hotkey.js（wysiwyg热键的配置文件，还支持拖拽上传文件）
③bootstrap.min.js（Boostrap支持）
④bootstrap-wysiwyg.js（wysiwyg的库文件）


2、使用方法

①初始化
$('#editor). wysiwyg();  

②设置编辑框样式
#editor {overflow:scroll; max-height:300px}  

③添加自己想要的功能
照搬官网的配置

④获取编辑框的内容

看了editor，是个div，用新的属性：contenteditable=“true”，使得div可以编辑，所以获得编辑框的内容就跟平时获取代码的方法一样，由于引入了jq，所以就直接用$('#editor').html();  
清除编辑框的方法，是$('#editor').cleanHtml();








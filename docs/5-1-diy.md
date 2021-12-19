#### 自定义Web蜜罐

> Web蜜罐样例

从以下地址下载HFish官方提供的自定义Web蜜罐模板
  
http://img.threatbook.cn/hfish/svc/service-demo.zip  

解压后获得index.html和portrait.js两个文件。  


> index.html文件中的代码功能

&lt;form&gt;中的代码明确了页面上账密表单的提交方式，具体利用方式参考下文“制作全新的登陆页面”
&lt;script&gt;中的代码明确了调用jsonp的方式


> portrait.js 文件中的代码功能

该文件是jsonp溯源功能的利用代码，攻击者在已登录其他社交平台的情况下，成功利用会让蜜罐获得部分社交平台的账号信息。

本代码因为利用了Chrome内核浏览器v80版本之前的漏洞，具有一定的时效性，随着攻击者更新自己的浏览器，利用代码可能失效，并有可能让攻击者在访问该页面时触发其杀毒软件报警。

您可以选择删除index.html中引用portrait.js的部分代码，或者自行优化portrait.js代码，补全更多反制方法。

HFish社区非常期待用户贡献漏洞利用代码。



#### 制作全新的登陆页面

用户还可以自己制作一个全新的登陆页面，通过替换表单元素实现“定制开发”

使用编辑器打开主页文件index.html，按照下面图片的提示修改表单元素。


![蜜罐web页面表格元素](http://img.threatbook.cn/hfish/20210728213641.png)



#### 打包并上传到蜜罐的管理后台

> 制作自定义蜜罐压缩包

把所有的静态文件文件打包名为“service-xxx.zip”文件，包括index.html 、portrait.js 以及其他所有格式的静态文件和文件夹。

`注意：文件命名为规范格式前缀 **必须** 为“service-”虽然用户可以修改“xxx”为适当的名字，但不能使用“web”和“root”字样，且压缩包 **必须** 为.zip格式。`

![image-20210508222121613](http://img.threatbook.cn/hfish/20210728213740.png)



> 上传自定义蜜罐压缩包

![image-20210508213915879](http://img.threatbook.cn/hfish/20210728213815.png)



> 配置新增服务页面

![image-20210508221316072](http://img.threatbook.cn/hfish/20210728213852.png)


如果一切正常，用户已经可以在【节点管理】和【模板管理】页面中使用该自定义蜜罐了。

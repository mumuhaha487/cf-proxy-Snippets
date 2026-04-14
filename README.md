<!-- Markdown提示/错误等：https://github.com/orgs/community/discussions/16925-->


<div align="center">
<h1>cf-proxy-Snippets</h1>

基于[cf-proxy-ex](https://github.com/1234567Yang/cf-proxy-ex)
</div>

# 原理 

可以部署在Snippets上，只需要压缩到32kb即可  
首先就是把js文件通过静态文件的方式进行上传  
这样就分为两个文件:  
-  一个主程序snippets.js，用于实现基本逻辑和框架  
-  一个js文件yproxy-client.js，用于被snippets引入

snippets.js用于填写到Cloudfare的snippets上。  
然后yproxy-client.js用于部署在静态网站上托管。(注意，要记得链接，然后修改snippets.js内容进行引入）

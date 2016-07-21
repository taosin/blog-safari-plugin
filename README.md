# 博客系统的safari插件
在我们的博客中，有一个功能叫'阅读轨迹'，其是专门用于罗列个人阅读过的文章。  
它的收录方式不是从CMS中去添加，而是利用Safari的插件，完成收录。
每次读到好文章的时候，只要点击地址栏左侧的![Alt text](http://carefree.oss-cn-shanghai.aliyuncs.com/fav.png)，输入标签，ok。这样我就可以在阅读文章的同时，轻松完成收录工作，不遗漏好文章。

**配置修改**
由于非常简单，用ajax调用后台api就可以完成收录工作，所以直接使用了jQuery。
用户在使用的时候，手动修改如下地方的代码为自己的api地址就可以了。

```
$.post('http://xxx/url', {
```
**操作方法**
用户下载该工程后，按照自己的需要修改配置，然后操作如下： 
> safari --> 开发 --> 现实扩展创建器 --> 点击左下'添加扩展' --> 选择到该工程 --> 左上出现myblog的扩展，点击它 --> 点击右上的'安装'按钮。

到此就可以在safari的扩展位置出现插件标示了，你就可以快乐的使用了。

forked from [Hades](https://github.com/iAmHades/blog-safari-plugin)

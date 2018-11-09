---
title: 轻松代建个人博客  Hexo+Github一步步搭建属于自己的博客
date: 2018-11-02 22:41:34
tags:
 - 博客搭建
---
<div class="post">
		<h1 class="postTitle">
			<a id="cb_post_title_url" class="postTitle2" >使用Hexo+Github一步步搭建属于自己的博客（基础）</a>
		</h1>
		<div class="clear"></div><div class="postBody">
		<div id="cnblogs_post_body" class="blogpost-body"><p>前言：电脑系统为window 10专业版，64位</p>
<p>&nbsp;</p>
<div id="cnblogs_post_body" class="blogpost-body"><p>欢迎预览
<a href="https://blog.malik.pub">我的博客</a>
</p>
<p>&nbsp;</p>
<p><strong>相关步骤：</strong></p>
<p>1、安装Node.js和配置好Node.js环境，打开cmd命令行，成功界面如下</p>

![成功界面](https://i.loli.net/2018/11/03/5bdd0d59741cc.png)
	
<p>&nbsp;2、安装Git和配置好Git环境，安装成功的象征就是在电脑上任何位置<strong>鼠标右键</strong>能够出现如下两个选择</p>




[![2.png](https://i.loli.net/2018/11/03/5bdd108881a7e.png)](https://i.loli.net/2018/11/03/5bdd108881a7e.png)
<p>注意：一般出于安全考虑，只有在Git Bash Here中才能进行Git的相关操作。如果需要在cmd命令行里调用Git，那么就要配置电脑的环境变量Path，或者在安装的时候选择use Git from the Windows Command Prompt。这个可有可无，影响不大，成功配置的界面如图</p>



[![3.png](https://i.loli.net/2018/11/03/5bdd10886dc35.png)](https://i.loli.net/2018/11/03/5bdd10886dc35.png)

<p>&nbsp;3、Github账户注册和新建项目，项目必须要遵守格式：账户名.github.io，不然接下来会有很多麻烦。并且需要勾选Initialize this repository with a README</p>
<p><img src="https://img-blog.csdn.net/20180705110531880?watermark/2/text/aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzM0MjkxNzc3/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70" alt=""></p>
<p>&nbsp;</p>

<p>在建好的项目右侧有个settings按钮，点击它，向下拉到GitHub Pages，你会看到那边有个网址，访问它，你将会惊奇的发现该项目已经被部署到网络上，能够通过外网来访问它。&nbsp;</p>
<p><img src="https://img-blog.csdn.net/20180705111356729?watermark/2/text/aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzM0MjkxNzc3/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70" alt=""></p>

<p>&nbsp;</p>
<p>&nbsp;4、安装Hexo，在自己认为合适的地方创个文件夹，我是在D盘建了一个blog文件夹。然后通过命令行进入到该文件夹里面</p>



[![4.png](https://i.loli.net/2018/11/03/5bdd1088604b4.png)](https://i.loli.net/2018/11/03/5bdd1088604b4.png)
<p>&nbsp;</p>
<p>输入npm install hexo -g，开始安装Hexo</p>


[![5.png](https://i.loli.net/2018/11/03/5bdd108892680.png)](https://i.loli.net/2018/11/03/5bdd108892680.png)
<p>&nbsp;</p>
<p>输入hexo -v，检查hexo是否安装成功</p>


[![6.png](https://i.loli.net/2018/11/03/5bdd10887242d.png)](https://i.loli.net/2018/11/03/5bdd10887242d.png)
<p>&nbsp;</p>
<p>输入hexo init，初始化该文件夹（有点漫长的等待。。。）</p>


[![7.png](https://i.loli.net/2018/11/03/5bdd108850f39.png)](https://i.loli.net/2018/11/03/5bdd108850f39.png)





<p>看到后面的“Start blogging with Hexo！”，激动有木有！！！！！</p>

[![8.png](https://i.loli.net/2018/11/03/5bdd1087ba600.png)](https://i.loli.net/2018/11/03/5bdd1087ba600.png)
<p>&nbsp;</p>
<p>输入npm install，安装所需要的组件</p>

[![9.png](https://i.loli.net/2018/11/03/5bdd1087bcf69.png)](https://i.loli.net/2018/11/03/5bdd1087bcf69.png)
<p>&nbsp;</p>
<p>输入hexo g，首次体验Hexo</p>

[![10.png](https://i.loli.net/2018/11/03/5bdd10888396f.png)](https://i.loli.net/2018/11/03/5bdd10888396f.png)
<p>&nbsp;</p>
<p>&nbsp;输入hexo s，开启服务器，访问该网址，正式体验Hexo</p>

![11.png](https://i.loli.net/2018/11/03/5bdd12baba6f5.png)


<p>问题：假如页面一直无法跳转，那么可能端口被占用了。此时我们ctrl+c停止服务器，接着输入“hexo server -p 端口号”来改变端口号</p>




![12.png](https://i.loli.net/2018/11/03/5bdd12bac85ea.png)

<p>那么出现如下图就成功了</p>

![-1.png](https://i.loli.net/2018/11/03/5bdd1333af3c8.png)

<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;5、将Hexo与Github page联系起来，设置Git的user name和email（如果是第一次的话）</p>



![13 (2).png](https://i.loli.net/2018/11/03/5bdd12bac8065.png)

```bash
$ git config  --global user.name "feng"
$ git config  --global user.email "邮箱名"
```

<p>上图是在其文件夹里面鼠标右键，点击Git Base Here。这里“feng”可以替换成自己的用户名，邮箱可以替换成自己的邮箱，这个地方必须是设置全局的，否则后面生成部署文章时会报错！</p>
<p>&nbsp;</p>
<p>输入cd ~/.ssh，检查是否由.ssh的文件夹</p>

![14.png](https://i.loli.net/2018/11/03/5bdd12baba15a.png)


<p>&nbsp;</p>
<p>输入ls，列出该文件下的内容。下图说明存在</p>

![15.png](https://i.loli.net/2018/11/03/5bdd12bad65c7.png)

<p>&nbsp;</p>


<p>&nbsp;输入ssh-keygen -t rsa -C “邮箱名”，连续三个回车，生成密钥，最后得到了两个文件：id_rsa和id_rsa.pub（默认存储路径是：C:<span class="hljs-command">\Users<span class="hljs-command">\Administrator<span class="hljs-command">\.ssh）</span></span></span>。</p>

<p>&nbsp;</p>
<p>&nbsp;输入eval "$(ssh-agent -s)",启动ssh-agent   ssh代理</p>



![16.png](https://i.loli.net/2018/11/03/5bdd12bae5172.png)
<p>&nbsp;</p>
<p>&nbsp;再输入ssh-add ~/.ssh/id_rsa，添加生成的SSH key到ssh-agent</p>



![17.png](https://i.loli.net/2018/11/03/5bdd12bae57f5.png)

<p>&nbsp;</p>
<p>&nbsp;登录Github，点击头像下的settings，添加ssh</p>

![18.png](https://i.loli.net/2018/11/03/5bdd12bc9d681.png)
<p>&nbsp;</p>
<p>新建一个new ssh key，将id_rsa.pub文件里的内容复制上去</p>
<p><img src="https://img-blog.csdn.net/20180705114102154?watermark/2/text/aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzM0MjkxNzc3/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70" alt=""></p>

<p>&nbsp;</p>
<p>输入ssh -T git@github.com，测试添加ssh是否成功。如果看到Hi后面是你的用户名，就说明成功了</p>



![19.png](https://i.loli.net/2018/11/03/5bdd18bf161b7.png)

<p><span style="color: #993300"><strong>问题：</strong></span>假如ssh-key配置失败，那么只要以下步骤就能完全解决</p>


<p>首先，清除所有的key-pair<br>ssh-add -D<br>rm -r ~/.ssh<br>删除你在github中的public-key</p>
<p>重新生成ssh密钥对<br>ssh-keygen -t rsa -C "xxx@xxx.com"</p>
<p>接下来正常操作<br>在github上添加公钥public-key:<br>1、首先在你的终端运行 xclip -sel c ~/.ssh/id_rsa.pub将公钥内容复制到剪切板<br>2、在github上添加公钥时，直接复制即可<br>3、保存</p>


测试：<br>在终端 ssh -T git@github.com


<p>&nbsp;</p>
<p>6、配置Deployment，在其文件夹中，找到_config.yml文件，修改repo值（在末尾）</p>
<p><font color=red size=5 face=“黑体”>注意这个地方有个坑</font>，第一打开_config.yml文件时type冒号与git之间竟然没有空格的，再说一遍没有空格呀！但是必须加上空格！！！这3个都要加上空格！！！</p>
<p>&nbsp;</p>

![这里写图片描述](https://img-blog.csdn.net/20180705113231624?watermark/2/text/aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzM0MjkxNzc3/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70)

<p>&nbsp;</p>

<p>repo值是你在github项目里的ssh（右下角）</p>


![这里写图片描述](https://img-blog.csdn.net/20180705113045514?watermark/2/text/aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzM0MjkxNzc3/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70)
<p>&nbsp;</p>
<p>如果这3个冒号之后有空格也有没有空格的，会报bad indentation of a mapping entry at line 82.......错误。我是没有注意到文件自带的type中没有空格，只有剩下两个加上了，报出这个错误。</p>
<p>如果这3个冒号都没有加上空格，不会报错，但是最后部署提交时，打开博客地址是与第一次创建项目一样，没有起到效果。因为hexo根本没有提交到所给git地址仓库中。</p>

---
<p>7、新建一篇博客，在cmd执行命令：hexo new post “博客名”</p>

![20.png](https://i.loli.net/2018/11/03/5bdd14bb6fd16.png)


<p>&nbsp;</p>
<p>&nbsp;这时候在文件夹_posts目录下将会看到已经创建的文件</p>


![-2.png](https://i.loli.net/2018/11/03/5bdd1936c2340.png)
<p>&nbsp;</p>
<p>在生成以及部署文章之前，需要安装一个扩展：npm install hexo<span class="hljs-attribute">-deployer<span class="hljs-attribute">-git <span class="hljs-subst">--save</span></span></span></p>

![扩展.png](https://i.loli.net/2018/11/03/5bdd1a0e79e1b.png)
<p>&nbsp;</p>
<p>使用编辑器编好文章，那么就可以使用命令：hexo d -g，生成以及部署了</p>

![22.png](https://i.loli.net/2018/11/03/5bdd14bb6ef9f.png)


<p>&nbsp;</p>
<p>部署成功后访问你的地址：http://用户名.github.io。那么将看到生成的文章，如果没有看到，前面都没有问题，查看git项目下的日期目录下有文章，说明是没有问题的，等待一会刷新就出来啦</p>

![这里写图片描述](https://img-blog.csdn.net/20180628112714447?watermark/2/text/aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzM0MjkxNzc3/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70)
![23.png](https://i.loli.net/2018/11/03/5bdd14bc6a4eb.png)
<p>&nbsp;</p>
<p>&nbsp;好了，到此为止，最基本的也是最全面的hexo+github搭建博客完结。接下来是进阶的操作</p>
<p>&nbsp;</p></div><div id="MySignature"></div>
<div class="clear"></div>
<div id="blog_post_info_block">
<div id="BlogPostCategory"></div>
<div id="EntryTag"></div>
<div id="blog_post_info"><div id="green_channel">
</div>
</div>
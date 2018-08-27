# github使用
> * github地址:[https://github.com/](https://github.com/)
> * 打开浏览器，访问GitHub，申请账号，如下图所示

![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/wgpTq5tQknRHQmzB4gga.oZ633H.7ul1BHvk3wBMv18!/b/dFoAAAAAAAAA&bo=2wNXAgAAAAARB70!&rf=viewer_4)

![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/EPJt2jzf6KdBFluPZ9mAfA7zPdckv8WN6qlejQ*4g5Y!/b/dDcBAAAAAAAA&bo=5APbAQAAAAARBw0!&rf=viewer_4)

![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/PBLl9y7CqWEQCLMLQtGTv3TgdnZiijPQIl0gio18Jj0!/b/dDUBAAAAAAAA&bo=ZANnAgAAAAARFyI!&rf=viewer_4)

![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/o628cSNkpv*yPKjooXmiq.h2.FEhQRVXQCx752kUFdw!/b/dDYBAAAAAAAA&bo=wQOTAQAAAAARF3A!&rf=viewer_4)

> * 新建仓库
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/4PO64WHsrSJshnQutNFk1iBrMfgpgvpZ6GdzG3.Ag*M!/b/dDYBAAAAAAAA&bo=9gOVAQAAAAARF0E!&rf=viewer_4)

![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/rfQ95.LN0NyayXJlXt85XDeap5VFBMMPHbrNedJLB5Q!/b/dDQBAAAAAAAA&bo=OgNRAgAAAAARB1o!&rf=viewer_4)

# 安装git
> * git下载地址:[https://git-scm.com/downloads](https://git-scm.com/downloads)
> > * 1>选择自己想要下载的系统版本
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/k2*g7DyBCxciVbg.TOKr3FFh6hA6Iqm3UvP9w68e*O8!/b/dDEBAAAAAAAA&bo=KQMeAQAAAAADBxc!&rf=viewer_4)
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/xYDVsqRwFqvR.l0k9NXT3cExaEkyhxXPBOqIweb5qTM!/b/dPMAAAAAAAAA&bo=WQPXAQAAAAADN54!&rf=viewer_4)
> > * 2>git安装步骤
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/43UzN*SHNvlQnpYx0LHHULi1ceFAPLDsE98h1Yv0Cvc!/b/dDUBAAAAAAAA&bo=VQM5AgAAAAADJ28!&rf=viewer_4)
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/O2T0emxF4gjW5XsResfevgZmkpE9ow4jWyrKwfNr55E!/b/dDQBAAAAAAAA&bo=RgMSAgAAAAADF2c!&rf=viewer_4)
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/ivvv54tKiVRcTztGYQN3lSrLomiQTJ6UC5p8aiFUEDk!/b/dDABAAAAAAAA&bo=ewP*AQAAAAADJ4Q!&rf=viewer_4)
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/HUE7c1z74PjbFmWAaAyyXWK82SIIuWek4p*E.koCC0I!/b/dDcBAAAAAAAA&bo=UQMfAgAAAAADJ00!&rf=viewer_4)
> > * 3>配置git
>  * 在用户主目录（C:\Users\Administrator）下，新建.ssh文件，如果有，再看文件下有没有id_rsa和id_rsa.pub这两个文件，如果已经有了，可直接到下一步。如果没有，打开Git Bash，输入命令，创建SSH Key；
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/qF.ztgBdh4fvX9Y*KfNTVXb3VVVSyaPjp7Fm*p.0a6g!/b/dDYBAAAAAAAA&bo=jQPDAgAAAAADN10!&rf=viewer_4)
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/B30nZmoYaKvnZ5Ewn87IIgCqneOqn2GyCTBr4hszjT8!/b/dDIBAAAAAAAA&bo=FQI5AAAAAAADFxw!&rf=viewer_4)
>  * 直接回车就哦了
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/fykuKbCAQfykC0KBQhzQU6O7lkQzaUhbzLgxRwQwqLc!/b/dFYAAAAAAAAA&bo=CAJ4AQAAAAADF0E!&rf=viewer_4)
>  * 出现上图，就说创建成功啦，再去用户主目录里找到.ssh文件夹，里面有id_rsa和id_rsa.pub两个文件，这两个就是SSH Key的秘钥对，id_rsa是私钥，不能泄露，id_rsa.pub是公钥，可以公开.接下来到GitHub上，打开“Account settings”--“SSH Keys”页面，然后点击“Add SSH Key”，填上Title（随意写），在Key文本框里粘贴 id_rsa.pub文件里的全部内容\
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/BBuHlNCLvN2mPN19yHiwWSgIjbVFivxp43I4FzFelEQ!/b/dDcBAAAAAAAA&bo=5gKaAQAAAAADF00!&rf=viewer_4)
>  * 点“Add Key”，你就应该看到已经添加的Key，可以添加多个Key
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/IxKqnRWyAj2iSNL8hroujCuQjm*ZSVS3cVV.ysJsYtU!/b/dDMBAAAAAAAA&bo=6wLcAAAAAAADFwc!&rf=viewer_4)
>  * 为了验证是否成功，在git bash下输入：
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/dpsa4dRkvFZvLf8ODAensyitgb*d6OpQVfefO*ijgms!/b/dDcBAAAAAAAA&bo=NAMpAAAAAAADFyw!&rf=viewer_4)
>  * 如果初次设置的话，会出现如下界面，输入yes 同意即可
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/kvFYD9yQlfqwuqQ9V9VQMrgWm.qFTxb0q5*O5KAEwIw!/b/dDUBAAAAAAAA&bo=kQKfAAAAAAADFz4!&rf=viewer_4)
>  * (或如果是第一次的会提示是否continue，输入yes就会看到：You've successfully authenticated, but GitHub does not provide shell access 。这就表示已成功连上github。
接下来我们要做的就是把本地仓库传到github上去，在此之前还需要设置username和email，因为github每次commit都会记录他们。)
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/VT8ZOAPGUCTtDE*80x989lGU0nPYmWmcjOit28PwvNs!/b/dFkAAAAAAAAA&bo=JQNUAAAAAAADF0A!&rf=viewer_4)
>  * 进入要上传的仓库，右键git bash，添加远程地址：
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/rsfBXRHbWW.pEGR5BryzD0.4PfKbunEEidYYNbQw9xA!/b/dC0BAAAAAAAA&bo=LAJHAAAAAAADB0s!&rf=viewer_4)
>  * 后面的yourName和yourRepo表示你再github的用户名和刚才新建的仓库，加完之后进入.git，打开config，这里会多出一个remote "origin"内容，这就是刚才添加的远程地址，也可以直接修改config来配置远程地址。创建新文件夹，打开，然后执行 git init 以创建新的 git 仓库。

# 上传本地项目到github
>  * 新建文件夹
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/fjT7xdR0KyhvlYQiVqMv6bznujZz7Rv0g0oMOR8LU60!/b/dDUBAAAAAAAA&bo=*wEEAQAAAAADB9k!&rf=viewer_4)
>  * 执行指令：git init
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/3.2v.VSRO1csdb6DZb7bS5EBfSDgNwj6IeuxVF*Sr.I!/b/dDIBAAAAAAAA&bo=sgFWAAAAAAADF9c!&rf=viewer_4)
>  * 文件夹终会生成.gif隐藏文件
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/U0DHVR2fby9fuDM9KUfk2bzoNnjy1t.9BBXHax1kLKg!/b/dC8BAAAAAAAA&bo=6wLYAAAAAAADFwM!&rf=viewer_4)
>  * 执行指令：git add +'你要提交的文件或文件夹'.
将所有文件添加到仓库
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/V1yBRbzKWZxrC1HCrLO9wDEKtaAXG.n4qaIcuTFTisc!/b/dDEBAAAAAAAA&bo=cAFBAAAAAAADBxI!&rf=viewer_4)
>  * 执行指令：git commit -m "提交文件" 双引号内是提交注释
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/qBSYnYnfSIogk5LxEDcYQCbQyklR4AgR.Gc6Lnilry0!/b/dDQBAAAAAAAA&bo=QAFWAAAAAAADFyU!&rf=viewer_4)

# 本地仓库和远程仓库同步
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/Y4TiZ.XkqKf7ymuZPhE7UH5J4tBPLKLawOsO83bNNXI!/b/dEQBAAAAAAAA&bo=hwS4AAAAAAADFwk!&rf=viewer_4)
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/rsfBXRHbWW.pEGR5BryzD0.4PfKbunEEidYYNbQw9xA!/b/dC0BAAAAAAAA&bo=LAJHAAAAAAADB0s!&rf=viewer_4)

# 上传本地代码
>  * 执行指令：git push -u origin master,然后githuby页面就能看见了
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/qQ3c*g6YLPybN0*hgDBTkin*Fvl1faaae9i7gHdWX*U!/b/dAgBAAAAAAAA&bo=wQF8AAAAAAADB54!&rf=viewer_4)
# 从远程仓库获取最新代码
>  * $git pull origin master:master(git pull <远程主机名> <远程分支名>:<本地分支名>)
# 将远程仓库克隆到本地
>  * 选择克隆到本地的位置，右键选择 git bash 
![cmd-markdown-logo](http://m.qpic.cn/psb?/V10wo3GU3cdwDX/qF.ztgBdh4fvX9Y*KfNTVXb3VVVSyaPjp7Fm*p.0a6g!/b/dDYBAAAAAAAA&bo=jQPDAgAAAAADN10!&rf=viewer_4)

>  * 输入命令 git clone git@github.com:用户名/仓库名.git
# 管理分支
>  * 创建分支
> > * $git branch 'name'  
>  * 切换分支
> > * $git checkout 'name'  
>  * 合并分支
> > * $git merge 'name'
>  * 删除分支
> > * $git branch -d 'name'
>  * 查看分支
> > * $git branch
>  * 创建+切换分支
> > * $git checkout -b 'name'


# 有可能出现的错误
>  * git commit -m ''上传不上去,原因是git默认为忽略大小写
> > * 解决办法:运行git config core.ignorecase false,关闭git忽略大小写配置
 






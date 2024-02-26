1. npm install -g hexo-cli                  全局安装hexo-cli
2. hexo init blog                                 安装 Hexo 完成后，请执行下列命令，Hexo 将会在指定文件夹中新建所需要的文件。
3. cd blog
4. npm install                                      安装依赖
最后一步，使用hexo s 启动，并访问http://localhost:4000/。


常用指令
1.init：初始化文件夹。如果没有设置 folder ，Hexo 默认在目前的文件夹建立网站。
hexo init blog
2.new：新建一篇文章，如果标题包含空格的话，请使用引号括起来。
hexo new "title"
3.generate：生成静态文件。
hexo generate
//该命令可以简写为：
hexo g
4.server：启动服务器。默认情况下，访问网址为： http://localhost:4000/。
hexo server
//简写为
hexo s
5.hexo deploy
6.version：显示 Hexo 版本。

一键部署
1.首先安装 hexo-deployer-git。
npm install hexo-deployer-git --save

2.第二步在_config.yml文件中添加配置。
deploy:
  type: git
  repo: https://github.com/yang-yyds/yang-yyds.github.io
  branch: master

3.第三步生成静态文件。
hexo g 或者 hexo generate

4.最后一步部署。
hexo d 或者 hexo deploy

部署完后，在Github查看上传的代码，并访问yang-yyds.github.io即可在线访问博客网站！

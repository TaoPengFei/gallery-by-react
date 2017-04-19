# gallery-by-react
one photo gallery project base on react

1、安装npm -g yo<br>
2、查看yeoman版本 yo —version<br>
3、安装generator ：npm install -g generator-react-webpack<br>
4、查看当前机器安装的grnerator版本:  npm ls -g --depth=1 2>/dev/null|grep generator-<br>

（1）npm ls -g :列出全局安装的所有npm包<br>
（2）--depth=1:树状结构最多向下展示一层<br>
（3）2>/dev/null: 如果执行npm ls -g的过程中，有错误消息，把错误消息重定向到我们的空设备文件上<br>
>表示重定向<br>
1表示standard out标准输出<br>
2表示standard error 标准错误<br>
/dev/null表示空设备文件<br>
（4）|表示通道，用来将上一个命令的输出内容作为下一个命令的输入内容<br>
（5）grep generator-:在前面的输出结果中，检索generator开头的关键字内容。<br>
5、新建的项目拉到本地<br>
（1）进入workspace,终端输入：git clone +项目地址<br>
（2）进入项目目录：cd gallery-by-react(项目名称)<br>
（3）终端输入：yo react-webpack gallery-by-react<br>
（4）提示是否需要react-router(y/n)，因为这里是单页面程序，不需要路由，所以选n<br>
（5）选sass<br>
（6）终端输入：grunt-serve，让我们的站点跑起来<br>


6、grunt dist 替换成 npm run dist<br>
sass-loader 依赖node-sass 需要安装node-sass<br>
7、查看git 状态 git status<br>
8、添加 git add -A<br>
   提交 git commit -m “说明”<br>
   push到github ：git push<br> 
9、需要先import ReactDOM from 'react-dom';才能使用ReactDOM.findDOMNode(this.refs.imgFigure0)<br>
10、cfg下是新版的配置信息<br>

<strong>项目安装运行</strong><br>
npm install<br>
npm start<br>
<strong>把项目发布到gh-pages分支</strong>
图片路径错误：<br>

将default.js 中的publicPath:'/assets/' 修改为 ’／gallery-by-react/assets/'<br>
![image](https://github.com/zhangxintong/gallery-by-react/raw/master/src/images/path.png)<br>

修改完后 执行 npm run dist<br>
先提交到master,命令如下：
git add .<br>
git commit -m "说明"<br>
git push<br>
提交到gh-pages分支<br>
git add dist<br>
git subtree push --prefix=dist origin gh-pages<br>


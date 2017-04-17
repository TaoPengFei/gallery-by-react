# gallery-by-react
one photo gallery project base on react

1、安装npm -g yo<br>
2、查看yeoman版本 yo —version<br>
3、安装generator ：npm install -g generator-react-webpack<br>
4、查看当前机器安装的grnerator版本:  npm ls -g --depth=1 2>/dev/null|grep generator-<br>
5、grunt dist 替换成 npm run dist<br>
sass-loader 依赖node-sass 需要安装node-sass<br>
6、查看git 状态 git status<br>
7、添加 git add -A<br>
   提交 git commit -m “说明”<br>
   push到github ：git push<br> 
8、需要先import ReactDOM from 'react-dom';才能使用ReactDOM.findDOMNode(this.refs.imgFigure0)<br>
9、cfg下是新版的配置信息<br>

<strong>项目安装运行</strong><br>
npm install<br>
npm start<br>
<strong>把项目发布到gh-pages分支</strong>
图片路径错误：<br>

将default.js 中的publicPath:'/assets/' 修改为 ’／gallery-by-react/assets/'<br>
![image](http://https://github.com/zhangxintong/gallery-by-react/blob/master/src/images/path.png)<br>

修改完后 执行 npm run dist<br>
先提交到master,命令如下：
git add .<br>
git commit -m "说明"<br>
git push<br>
提交到gh-pages分支<br>
git add dist<br>
git subtree push --prefix=dist origin gh-pages<br>

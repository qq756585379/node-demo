先手动在node-demo目录下创建src文件夹和README文件

1. 命令行创建npm的配置文件，在node-demo目录下打开命令窗口
 - a. npm init --yes 自动生成package.json默认配置。

2. 添加一个gulp的依赖
 - a.（如果未下载全局gulp,先下载全局gulp）npm install -g gulp
 
 - b. 在node-demo目录下 npm install gulp --save-dev 这样就把gulp写进项目package.json文件依赖中，别人直接clone代码后直接npm install就会自动把package.json中依赖的文件下载到他的本地。

3. 在项目根目录下添加一个gulpfile.js文件，这个是gulp的主文件，这个文件名是固定的。

4. 在gulpfile中抽象我们需要做的任务，在gulpfile里需要用到很多插件，我们得一个一个下载安装,用到哪些就得下载哪些
>npm install gulp-less --save-dev
>
>npm install gulp-concat --save-dev
>
>npm install gulp-uglify --save-dev
>
>npm install gulp-cssnano --save-dev
>
>npm install gulp-htmlmin --save-dev
>
>npm install browser-sync --save-dev

5.写完gulpfile文件后我们就执行gulpfile里的方法，gulp serve就会监听src下的所有文件变化，并同步到dist文件夹下。

6.下面配置git。

zzaiixnsicsicijdid


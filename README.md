# bfm-model

> 

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```
##安装的插件和依赖
```bash
#sass安装
cnpm install node-sass --save-dev //安装node-sass 
cnpm install sass-loader --save-dev //安装sass-loader 
cnpm install style-loader --save-dev //安装style-loader 有些人安装的是 vue-style-loader 其实是一样的！
# webpack-base.config.js中配置
{ 下面需要你手动添加，相当于是编译识别sass! 
   test: /\.scss$/,
   loaders: ["style", "css", "sass"]
} 
<style lang="scss" scoped="" type="text/css"> 
//你的sass语言 $primary-color: #333; 
  body {
    color: $primary-color; //编译后就成了 color:#333;类似于js的变量！ 
    } 
</style>



For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

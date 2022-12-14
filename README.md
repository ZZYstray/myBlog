# VUE-Tangyida's BLOG

> Tangyida's blog based on Vue.js。基于vue+webpack的个人博客模板

## 前言

大概花2周的时间把自己的博客整理了一下，把各个组件抽取了出来，做成了一个通用博客的模板。

在这你可以写自己的技术文章，也可以记录自己的生活点滴，也可以向别人展示自己。

整个博客模板是基于[Vue.js](https://cn.vuejs.org/)+[webpack](https://www.webpackjs.com/)开发的，这是一份单页面的项目（PS：所有的数据和图片等等都是测试的，我随机放上去的，无任何网络请求）。


## 预览

#### 一、主页


#### 二、博客列表


#### 三、生活版面
#### 四、博文详细



#### 五、关于我，留言


## 开始

``` bash
# 安装所有的依赖
npm install

# 在本地localhost:8081运行开发环境
npm run dev

# build你的工程
npm run build
```

## 项目结构

### 文件结构

```javascript
|——build // 这里是放build的配置，包括vue项目本身的配置和webpack打包的配置
|——config // 这里是一些基本的项目配置
|——static
| |——bootstrap // 这里放你需要外部引用的js，当然你通过添加依赖也可以
| |——jquery
|——src
| |——assets // 这里放你需要的一些资源(本地图片，css，js，测试文章等)
| |——config // 这里是整体项目数据的存放点，也就是配置项
| |——router // 路由的配置
| |——utils // 所有工具类的通用js
| |——views // 所有页面
|  |——cores // 主页面
|  |——components // 页面其他所有组件
```

### 页面架构

我把整体的页面架构从两个入口页面着手：

- entry.vue
- detail.vue

### 入口页面

####  #entry.vue

这是四个路由（/，/blog，/life，/contact）四个页面的公用组件页面。头部和顶部导航栏是公用的。

route-view对应接下来的四个（在文件夹cores里面的主页面），分别是index（主页），blog（博文页面），life（生活板块），contact（关于我）的构造。

####  #detail.vue

这是两个页面（/detail，/detail/life）的公共组件页面。头部和文章标题等详细介绍是公用的。

两个页面：/detail（文章详细），/detail/life（生活详细）分别由上面构造。

以上是页面的整体架构。

## 组件

（未完待续）

## 配置项

（未完待续）


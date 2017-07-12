# Vue-development-pit-trip--1

vue-router 里面的mode配置

注意这里使用的vue-router 2.x

const router = new Router({
  mode: 'history',
  base: __dirname,
  routes
})
本问题主要解决于使用vue2.x开发app内嵌页面等场景

如果我们正常开发一个单页面应用都是有入口页面的，所以说不存在此问题，但是 当我们打包好的静态文件，直接启动服务是可以访问 localhost:8080，而访问localhost:8080/news却是报错，

此时把上面的配置 mode：history改为hash就可以了，只不过url看起来稍微不是很美观

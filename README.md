### electron
[http://www.electronjs.org/docs/tutorial/quick-start](http://www.electronjs.org/docs/tutorial/quick-start)

[https://github.com/electron/electron](https://github.com/electron/electron)

[BrowserWindow](https://cloud.tencent.com/developer/section/1115971)

### electron + vue
<del>Electron+vue的使用</del>: [https://www.jianshu.com/p/839362c64bdb](https://www.jianshu.com/p/839362c64bdb) 

**Electron+Vue 项目搭建** : [https://blog.csdn.net/gswwxyhk/article/details/109910009](https://blog.csdn.net/gswwxyhk/article/details/109910009)

```
vue init simulatedgreg/electron-vue my-project
```

### electron-vue
if `npm install electron` failed, use `cnpm` try again.

[https://simulatedgreg.gitbooks.io/electron-vue/content/cn/](https://simulatedgreg.gitbooks.io/electron-vue/content/cn/)

[https://github.com/SimulatedGREG/electron-vue](https://github.com/SimulatedGREG/electron-vue)
```
# Install vue-cli and scaffold boilerplate
npm install -g vue-cli
vue init simulatedgreg/electron-vue my-project

# Install dependencies and run your app
cd my-project
yarn # or npm install
yarn run dev # or npm run dev
```

在webpack.renderer.config.js 和 webpack.web.config.js中添加
```
  templateParameters(compilation, assets, options){
    return {
      compilation: compilation,
      webpack: compilation.getStats().toJson(),
      webpackConfig: compilation.options,
      htmlWebpackPlugin: {
        files: assets,
        options: options
      },
      process,
    };
  }
```
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210209180147619.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzI2MjY3Mzg1,size_16,color_FFFFFF,t_70)
### electron-vuex
[https://github.com/vue-electron/vuex-electron](https://github.com/vue-electron/vuex-electron)

[https://github.com/vue-electron/vuex-electron-example](https://github.com/vue-electron/vuex-electron-example)

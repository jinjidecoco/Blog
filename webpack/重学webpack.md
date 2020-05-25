#### 重学webpack 

##### 1.开始 

`yarn  webpack webpack-cli -D `

![image-20200411154033590](/Users/coco/Library/Application Support/typora-user-images/image-20200411154033590.png)

##### 新建 src/index.js 里面随便放点内容

`npx webpack --mode=development` webpack 默认是 `production` 模式

默认入口 `./src` 打包完成到 `dist/main.js`

##### 2. 新建立webpack.config.js

注意loader要配置在`module.rules` 里，rules是一个数组

##### use的用法

1. 可以是字符串 `use:'babel-loader'`

2. 可以是数组 `use:['style-loader','css-loader']`

3. 可以是对象 

   ```js
    use:{ 
   		loader:'babel-loader',
   		options{ }
    }
   ```

   

我们在打包时的设置了--mode,其实可以在 直接在webpack.config.js 里配置  `mode: "development",`

##### 4.查看页面

新建public目录，其下建立 `index.html`

安装 `yarn add html-webpack-plugin -D` 

##### 5.浏览器展示

`yarn add webpack-dev-server -D`













## 动机

就是样式好看 规范样式前提下 行为层（js可自行封装 务必使dom层与js分离 减少耦合）


## 链接
原组件官网链接
* [官方文档](https://ksc-fe.github.io/kpc/)
* [Intact MVVM框架][1]
* [Vdt 模板引擎](http://javey.github.io/vdt.js/)
* [Intact-Vue 兼容层](https://github.com/Javey/intact-vue)
* [Intact-React 兼容层](https://github.com/ksc-fe/intact-react)


## 开发

```shell
git clone https://github.com/3twork/component.git
cd component
npm install
npm run dev:doc

# 测试
npm run test
# 更新测试快照
npm run snapshot
# 部署文档
npm run deploy:doc
# 发版
npm run release
```

## 二次开发

请自行抽离styles文件下的stylus 然后与日常脚手架结合生成xxx.css 引入项目中
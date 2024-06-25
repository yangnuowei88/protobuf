# vue-protobuf

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```
## 项目的一些说明
- 并没有全局去按照这个，实际上是按照了protojS 这个里面就自带了他的呀

- **其中./pbjs 在node_module的./bin中**
- JSON的这种基本不会用的哈，虽然是等价的
- proto 这句话的意思是吧**所有的指定目录的proto目录文件**，转译到proto.js文件里面去

```shell
    
  "proto:json": "pbjs -t json src/proto/*.proto > src/proto/proto.json", 
  "proto": "pbjs -t json-module -w commonjs -o src/proto/proto.js  src/proto/*.proto"



```
## 原文连接
[如何在前端中使用protobuf（vue篇)](https://juejin.cn/post/6844903699458818062?searchId=202406211648301E1D05C96BE9E88E8F0A)

## 开发说明

### 目录结构
详见[目录结构](目录结构.md)

### 环境
1. node 大于v10.0.0

### 编译运行
```bash
  # 开发模式
  npm run dev # 编译并输出至2.x目录
  npm run dev -- -t 1.x # 编译并输出至1.x目录
  npm run dev -- -t 1.x,2.x # 编译并输出至1.x目录和2.x目录
  
  # 生产模式
  npm run build # 编译并输出至2.x目录
  npm run build -- -t 1.x # 编译并输出至1.x目录
  npm run build -- -t 1.x,2.x # 编译并输出至1.x目录和2.x目录
```

### 生成文档
```bash
  npm run doc
```

### 发布
1. 修改package.json中版本号
```js
  //package.json
  {
    //...
    "version-1.x": "1.0.17", //要发布1.x版本，修改此处
    "version-2.x": "2.0.0",  //要发布2.x版本，修改此处
    //...
  }
```
2. 发布
```bash
  # 发布
  npm run pub # 发布1.x版本和2.x版本
  npm run pub -- -t 1.x # 发布1.x版本
  npm run pub -- -t 2.x # 发布2.x版本
```
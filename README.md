# 前端应用构建部分

## 程序说明

> 利用npm搭建一个基于json-server的、提供后端（json文件型）数据库访问的Restful API服务器；然后使用Ajax异步调用技术编写一个前端应用程序，通过调用上述Restful API服务器提供的数据访问接口，实现对后端数据库的增、删、改、查功能。

### 文件

```bash
.
|-- README.md // 说明文档
|-- db.json // json-server 数据库文件
|-- staic
|   `-- css
|       |-- Register.css  
|       `-- style.css // 样式文件
`-- templates
    |-- add.html // 增
    |-- delete.html // 删
    |-- index.html // 主页
    |-- query.html // 查
    `-- update.html // 改

3 directories, 9 files
```

### 搭建和启动json-server

1. 初始化一个工作目录

```bash
npm init
```

2. 安装json-server

```bash
npm install --save json-server
```

3. 打开`package.json`
4. 删除"scripts"项目,添加

```json
"scripts": {
    "json:server": "json-server --watch db.json --port 3000"
  },
```
5. 运行json-server

```bash
npm run json:server
```
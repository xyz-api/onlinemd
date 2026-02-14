https://xyz-api.github.io/docs/

# 在线文档

静态 Markdown / PDF 阅读器，无需后端。

## 添加文档

1. 在 `biji/` 下新建文件夹，放入 `index.md` 或 `index.pdf`
2. 编辑 `folders.js`，添加一条记录：

```js
{ name: '显示名称', path: 'biji/文件夹名', type: 'md' }   // Markdown
{ name: '显示名称', path: 'biji/文件夹名', type: 'pdf' }  // PDF
```

## 目录结构

```
biji/
  文档名/
    index.md    ← Markdown 文档（图片放同目录）
    index.pdf   ← PDF 文档
folders.js      ← 文档索引
index.html      ← 页面入口
libs/           ← 前端依赖（marked、pdf.js、jszip）
```

## 运行

任意静态服务器托管根目录即可，或直接双击 `start.cmd`。

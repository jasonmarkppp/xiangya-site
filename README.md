# 想芽 · 把想法慢慢养成真的

**想芽** 是一个网页应用，帮你把脑子里的小念头整理、灌溉、慢慢养成真的。

## 线上访问

https://jasonmarkppp.github.io/xiangya-site/

## 技术栈

- React + Vite + TypeScript
- Tailwind CSS
- React Router（HashRouter）

## 本地运行

本仓库存放的是**构建后的静态产物**（`index.html` + `assets/`），可直接用任意静态服务器预览：

```bash
# 方式一：npx 起一个静态服务器
npx serve .

# 方式二：Python
python -m http.server 8080
```

然后打开 http://localhost:8080 即可。

## 更新部署

源码在 `xiangya-web` 工程中，每次改完代码后：

1. `npm run build` 构建
2. 将 `dist/` 下的产物（`index.html`、`assets/`、`favicon.svg`）复制到本目录
3. 提交并推送：

```bash
git add .
git commit -m "update: ..."
git push
```

推送后 GitHub Pages 会自动重新部署（约 1 分钟）。

## License

© 想芽 · All rights reserved.

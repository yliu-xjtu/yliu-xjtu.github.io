如果 GitHub Actions 还是不工作，你可以手动构建和部署：

> 注意：站点需要由 Hugo 构建并发布到 Pages。请不要在仓库根目录放置手写 `index.html`/`site.html`，否则会覆盖 Hugo 的最终页面。

## 本地构建
hugo --minify

## 然后将 public/ 目录的内容推送到 gh-pages 分支
git checkout -b gh-pages
cp -r public/* .
git add .
git commit -m 'Deploy Hugo site'
git push origin gh-pages

## 然后在 GitHub Pages 设置中选择 'gh-pages' 分支

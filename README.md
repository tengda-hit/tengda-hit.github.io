# Hugo 个人博客

## 本地预览

安装 Hugo 后运行：

```bash
hugo server -D
```

浏览器打开 <http://localhost:1313/>。

## 发布到 GitHub Pages

1. 把 `hugo.toml` 中的 `tengda-hit` 改成你的 GitHub 用户名。
2. 创建名为 `你的用户名.github.io` 的 GitHub 仓库。
3. 执行：

```bash
git init
git add .
git commit -m "建立 Hugo 博客"
git branch -M main
git remote add origin https://github.com/tengda-hit/tengda-hit.github.io.git
git push -u origin main
```

4. 在仓库的 **Settings → Pages → Source** 选择 **GitHub Actions**。
5. 等待 Actions 完成后访问 `https://你的用户名.github.io/`。

以后只需把 Markdown 文章放进 `content/posts/`，提交并 push，网站会自动更新。

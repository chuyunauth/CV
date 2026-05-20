# 📄 在线简历 - GitHub Pages

这是一个基于 GitHub Pages 托管的在线简历页面，打开链接即可直接查看 PDF 简历。

## 🚀 快速部署

### 方法一：个人主页 (`<username>.github.io`)

```bash
# 1. 创建 GitHub 仓库，命名为 <你的用户名>.github.io
# 2. 在本地初始化仓库
git init
git add .
git commit -m "初始化简历页面"
git branch -M main
git remote add origin https://github.com/<用户名>/<用户名>.github.io.git
git push -u origin main
```

### 方法二：项目页面

1. 在 GitHub 上创建一个仓库（如 `resume` 或 `CV`）
2. 推送代码到 `main` 分支
3. 进入仓库 Settings → Pages → 选择 `Deploy from branch: main`，根目录 `/`
4. 等待几分钟，即可通过 `https://<用户名>.github.io/<仓库名>/` 访问

## 📁 文件结构

```
.
├── index.html       # 主页面（PDF 查看器）
├── resume.pdf       # 你的简历 PDF 文件
├── _config.yml      # GitHub Pages 配置
└── README.md        # 本文件
```

## ✏️ 自定义

- **替换简历**：将新的 PDF 文件覆盖 `resume.pdf` 即可
- **修改标题**：编辑 `index.html` 中的 `<title>` 和页面标题文字
- **自定义域名**：添加 `CNAME` 文件，内容为你的域名

## 📝 注意事项

- PDF 文件建议控制在 10MB 以内以保证加载速度
- 推荐使用主流浏览器（Chrome、Edge、Firefox、Safari）查看
- 移动端自动适配

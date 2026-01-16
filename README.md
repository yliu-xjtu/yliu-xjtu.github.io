# 刘杨 - 个人学术主页

基于 Hugo 和 PaperMod 主题构建的学术个人网站。

## 访问地址

https://yliu-xjtu.github.io

## 技术栈

- **静态网站生成器**: Hugo
- **主题**: PaperMod
- **托管平台**: GitHub Pages

## 本地开发

### 1. 安装 Hugo

Windows:
```powershell
choco install hugo-extended -y
```

macOS:
```bash
brew install hugo
```

### 2. 本地预览

```bash
cd yliu-xjtu.github.io
hugo server -D
```

访问 http://localhost:1313

### 3. 构建生产版本

```bash
hugo --minify
```

## 内容管理

### 添加/修改论文

编辑 `data/publications.yml` 文件，遵循以下格式：

```yaml
journals:
  - title: "论文标题"
    authors: "作者列表"
    journal: "期刊名称"
    year: 2024
    type: "论文类型"
    google_scholar: true
```

### 添加/修改页面

编辑 `content/` 目录下的 Markdown 文件。

## 部署

推送到 main 分支后，GitHub Actions 会自动构建并部署到 GitHub Pages。

## 目录结构

```
yliu-xjtu.github.io/
├── config.yml              # 主配置
├── content/                # 页面内容
│   ├── _index.md          # Home
│   ├── home/              # 个人主页
│   ├── publications/      # 科研成果
│   ├── tools/             # 常用工具
│   └── students/          # 招生培养
├── data/                   # 数据文件
│   └── publications.yml   # 论文数据
├── static/                 # 静态资源
│   └── images/            # 图片
├── assets/                 # 资源文件
│   └── css/               # 自定义样式
└── themes/                 # 主题
    └── PaperMod/          # PaperMod 主题
```

## 联系方式

- Email: yangliu@xjtu.edu.cn
- 个人主页: https://gr.xjtu.edu.cn/web/yangliu/

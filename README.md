# Personal Blog

这是我的个人技术博客仓库，使用 GitHub Pages 部署。

## 项目说明 | Project Description

这个仓库包含了我的个人博客文章和技术分享。主要关注以下领域：
- 技术文章
- 学习笔记
- 项目经验分享
- 编程心得

## 部署说明 | Deployment

本博客使用 GitHub Pages 部署，访问地址：[待补充]

### 本地开发 | Local Development

1. 克隆仓库
```bash
git clone [your-repo-url]
cd blog
```

2. 安装 Hugo (推荐使用 extended 版本)[安装说明](https://hugo.opendocs.io/installation/linux/)
```bash
# Linux 安装
wget https://github.com/gohugoio/hugo/releases/download/v0.145.0/hugo_extended_0.145.0_linux-amd64.tar.gz 
tar -xvzf hugo_extended_*.tar.gz
sudo mv hugo /usr/local/bin/
```

1. 创建新站点 (如果尚未初始化)
```bash
hugo new site . --force
```

1. 添加主题 (以 loveIt 主题为例 tag 0.3.0)
[所有主题](https://themes.gohugo.io/)
```bash
git submodule add https://github.com/dillonzq/LoveIt.git themes/loveit
echo "theme = 'LoveIt'" >> hugo.toml
```

1. 本地预览
```bash
hugo server 
```

### GitHub Actions 自动化部署（推荐）

1. **创建工作流文件**：
   在 `.github/workflows/hugo.yml` 添加：
   ```yaml

   ```

2. **触发部署**：
   ```bash
   git push origin blog  # 推送后自动触发
   ```
3. **查看效果**

地址 https://eviljoker.github.io/blog/

### 手动部署（备选）


## 内容同步 | Content Sync

本博客内容会同步发布到以下平台：
- 掘金：[待补充个人主页链接]
- GitHub Pages：[待补充博客地址]

## 文章结构 | Content Structure

```
blog/
├── posts/          # 博客文章
├── assets/         # 静态资源
└── drafts/         # 草稿箱
```

## 贡献 | Contributing

欢迎提出建议和意见！可以通过以下方式：
1. 提交 Issue
2. 创建 Pull Request

## 许可证 | License

本项目采用 MIT 许可证 - 详见 [LICENSE](LICENSE) 文件

---

## 待办事项 | TODO
- [x] 配置静态站点生成器（Hugo）
- [x] 实现博客主题（LoveIt）
- [x] 配置自动部署
- [ ] 编写第一篇博客文章
- [ ] 设置评论系统
- [ ] 添加订阅功能 
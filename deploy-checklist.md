# LLMs.txt Generator — 部署检查清单

## 部署前准备

- [ ] 确保 `index.html` 能正常在本地打开运行
- [ ] 测试所有按钮功能：Generate、Copy、Download、Load Sample、Clear
- [ ] 确认移动端布局正常

---

## 部署后必做事项

### 1. 替换 Canonical URL
在 `index.html` 中搜索并替换：
```
#TO-BE-REPLACED-WITH-REAL-URL
```
替换为实际部署的域名，例如：`https://llms-txt-generator.example.com/`

### 2. 替换 Sitemap 域名
更新以下两个文件中的 `example.com`：

**sitemap.xml：**
```xml
<loc>https://your-actual-domain.com/</loc>
```
当前是单页站，sitemap 只保留首页。不要把 `#tool`、`#faq` 这类页面锚点作为独立 URL 放进 sitemap。

以及 `robots.txt` 中的 Sitemap 行：
```
Sitemap: https://your-actual-domain.com/sitemap.xml
```

**llms.txt（本站介绍文件）：**
更新所有 `https://example.com` 为实际域名。

### 3. 提交 Google Search Console
1. 登录 [Google Search Console](https://search.google.com/search-console)
2. 添加域名或 URL prefix 属性
3. 下载 HTML 验证文件并上传到网站根目录（如果使用域名验证）
4. 验证通过后提交 `sitemap.xml`
5. 使用 URL 检查工具请求首页索引

### 4. 请求索引
在 Google Search Console 中：
- 提交 `sitemap.xml` 后等待 1-2 天
- 使用"请求索引"功能对首页进行快速抓取
- 检查覆盖率报告，确保没有抓取错误

### 5. 添加 Cloudflare Web Analytics（如适用）
如果部署在 Cloudflare Pages：
1. 进入 Cloudflare Dashboard → Analytics
2. 找到 Web Analytics 选项
3. 添加网站并获取分析代码
4. 将分析代码添加到 `index.html` 的 `<head>` 底部

如果部署在其他平台，可选：
- Google Analytics 4
- Plausible Analytics
- Fathom

### 6. 社交分享

**X (Twitter)：**
- 撰写简洁的推广推文
- 包含工具链接和主要功能特点
- 可配截图或 GIF 演示

**Indie Hackers：**
- 在"Show off your project"板块发帖
- 说明解决了什么问题
- 强调免费、无需登录

**Reddit：**
- 相关子版块：
  - r/SideProject
  - r/webdev
  - r/SEO
  - r/Entrepreneur
- 不要 spam，专注于提供价值

**GitHub（如已创建仓库）：**
- 创建 Release
- 更新 README 中的链接
- 在相关社区分享

### 7. 记录第一周指标

建议记录的指标：

| 指标 | 记录日期 | 第1天 | 第3天 | 第7天 |
|------|----------|-------|-------|-------|
| 独立访客 (UV) | | | | |
| 页面浏览量 (PV) | | | | |
| 平均停留时间 | | | | |
| 跳出率 | | | | |
| 生成次数（可加事件追踪） | | | | |
| 复制按钮点击 | | | | |
| 下载按钮点击 | | | | |

**工具推荐：**
- Google Search Console（搜索流量）
- Cloudflare Analytics（独立访客）
- Google Analytics 4（深度行为数据）

---

## 后续优化

- [ ] 监控搜索关键词（Search Console）
- [ ] 分析用户行为（跳出率高的页面需优化）
- [ ] 收集用户反馈
- [ ] 考虑添加"邮箱收集"机制用于付费报告变现
- [ ] 根据数据决定下一个工具方向

---

## 注意事项

⚠️ **llms.txt 是实验性实践** — 这是新兴做法，不保证立即效果。专注于提供优质工具和内容，SEO 效果需要时间积累。

⚠️ **不要承诺排名提升** — 只说"帮助 AI 系统理解网站结构"，避免使用"保证提高排名"等表述。

---

最后更新：2026-06-24

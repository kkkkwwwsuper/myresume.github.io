# 秦泽慧 PettiChat 网页版简历

这是一个纯静态网页，不需要安装依赖或运行后端服务。主要文件：

- `index.html`：网页结构
- `styles.css`：页面样式和打印样式
- `script.js`：能力板块交互与作品数据弹窗
- `assets/douyin-evidence.jpg`：社媒作品数据截图
- `assets/秦泽慧-PettiChat北美社媒运营实习生-简历.pdf`：可直接作为邮件附件的 PDF 版本

## 本地查看

直接双击 `index.html`，或在本文件所在目录运行：

```powershell
Start-Process .\index.html
```

## 发布到 GitHub Pages

### 方式一：用 Git 命令上传

1. 在 GitHub 新建一个 **Public** 仓库，例如 `petitchat-resume`。
2. 不要勾选自动生成 README、`.gitignore` 或 License。
3. 在本文件夹打开 PowerShell，依次运行：

```powershell
git branch -M main
git add .
git commit -m "Add PettiChat resume website"
git remote add origin https://github.com/你的GitHub用户名/petitchat-resume.git
git push -u origin main
```

4. 打开 GitHub 仓库的 **Settings → Pages**。
5. 在 **Build and deployment** 中选择 **Deploy from a branch**。
6. Branch 选择 `main`，目录选择 `/(root)`，点击 **Save**。
7. 等待约 1-3 分钟，访问：

```text
https://你的GitHub用户名.github.io/petitchat-resume/
```

### 方式二：直接在 GitHub 网页上传

1. 新建一个 Public 仓库。
2. 进入仓库后点击 **Add file → Upload files**。
3. 把 `index.html`、`styles.css`、`script.js`、`.nojekyll`、`assets` 文件夹和本说明一起拖进去。
4. 点击 **Commit changes**。
5. 按上面的步骤进入 **Settings → Pages**，选择 `main` 和 `/(root)`。

## 邮件发送建议

推荐正文中放网页链接，并附上 PDF：

```text
主题：应聘 PettiChat 北美社交媒体运营实习生｜秦泽慧

您好，

我是秦泽慧，现为临床医学专业 2027 届本科生，申请 PettiChat 北美社交媒体运营实习生。
我有英文日常沟通、海外客户询盘处理、短视频内容运营和用户互动经验，其中单条作品获得 34.4 万播放。

在线互动简历：https://你的GitHub用户名.github.io/petitchat-resume/
PDF 简历见附件，期待有机会进一步沟通。

秦泽慧
18763176811｜18763176811@163.com
```

不要直接发送整个文件夹或压缩包。HR 端最方便的格式是“PDF 附件 + GitHub Pages 在线链接”。

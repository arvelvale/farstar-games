# 远星游戏工作室 · Farstar Games

远星游戏工作室（Farstar Games）的官方静态主页与品牌资产仓库，参考 `tidyhome` 的纯静态 GitHub Pages 方式构建，无第三方请求与追踪脚本。

## 目录与文件说明

| 文件 | 用途 |
| :--- | :--- |
| `logo-icon-512.png` | **推荐上传 TapTap**：去掉原图底部文字、重新居中并留安全边距的 `512 × 512` PNG 纯图标版 |
| `logo-with-text-512.png` | **备用对比**：原图带「远星游戏工作室 / FARSTAR GAMES」文字的 `512 × 512` PNG 缩放版 |
| `site/index.html` | 工作室主页（中英双语、介绍 + 《火柴三国：群英传》展示 + 联系方式） |
| `site/privacy.html` | 隐私政策占位页（供 TapTap 后续游戏创建及合规页面链接） |
| `site/logo.png` | 网页图标（与 `logo-icon-512.png` 一致） |
| `site/game-sanguo-icon.png` | 《火柴三国：群英传》图标（取自 `videos/sanguo/game/icon-512.png`） |
| `site/og.png` | `1200 × 630` 社交分享预览图 |
| `site/fonts/` | 自托管字体文件（Geist + Noto Sans SC，附 OFL 许可） |
| `.github/workflows/pages.yml` | 推送 `main` 时自动检查并部署 `site/` 到 GitHub Pages |

## 发布到 GitHub Pages（4 步上线）

1. 在 GitHub（账号 `arvelvale`）新建一个 **Public** 仓库，推荐命名 `farstar-games`。
2. 在本目录执行推送（或先确认 git 用户信息后再提交）：
   ```powershell
   git init -b main
   git add .
   git commit -m "初始化远星游戏工作室官网与 512x512 徽标"
   git remote add origin https://github.com/arvelvale/farstar-games.git
   git push -u origin main
   ```
3. 打开 GitHub 仓库的 **Settings → Pages**，将 **Build and deployment → Source** 选为 **GitHub Actions**。
4. 等待 Actions 跑完后，确认 **`https://arvelvale.github.io/farstar-games/`** 可正常打开，再填入 TapTap 厂商资料的「厂商网址」。

## TapTap 厂商资料可直接填写的参考字段

- **厂商 Logo**：上传 `logo-icon-512.png`（`512 × 512` PNG）
- **厂商别名**：`Farstar Games`
- **厂商网址**：`https://arvelvale.github.io/farstar-games/`
- **厂商简介**（精简版，约 140 字）：

> 远星游戏工作室（Farstar Games）是一家由个人独立开发者创立的游戏工作室，专注于动作格斗手感、横版无双玩法与小型创意互动体验。目前主力开发《火柴三国：群英传》，持续打磨招式连段、识破弹反与多武将战斗体验，以小步迭代做出扎实好玩的作品。

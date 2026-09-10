# 本地预览与发布

本版进一步参考 sun0225SUN/sun0225SUN：添加昼夜编程插画、动态分隔线、徽章、贡献贪吃蛇、3D 贡献城市、贡献趋势图和人物插画，保留太空主题和彩蛋。不包含当前项目介绍。

## 本地预览

在 VS Code 打开 README.md，按 Ctrl + Shift + V。网络图片需要联网。最终 GitHub 排版需发布后确认。折叠彩蛋使用 details/summary，终端文字是趣味文案，不执行命令。

## 发布

发布 README.md、.github、profile-snake-contrib、profile-3d-contrib 和 SETUP.md 到公开仓库 xiaozhaoben/xiaozhaoben 的默认分支。本版不依赖 assets 目录，旧图保留作备份。

```powershell
git add README.md SETUP.md .github/workflows/profile-visuals.yml profile-snake-contrib profile-3d-contrib
git commit -m "feat: 改版趣味太空主题个人主页"
git push -u origin HEAD
```

若使用 SSH，可执行：
`git remote set-url origin git@github.com:xiaozhaoben/xiaozhaoben.git`

## 视觉来源

- 动态标题与页尾：https://github.com/kyechan99/capsule-render
- 循环打字：https://github.com/DenverCoder1/readme-typing-svg
- 星云图片：https://images.nasa.gov/details/carina_nebula
- 图片署名：NASA / ESA / CSA / STScI

贡献图工作流在首次推送该工作流文件后运行，也可以从 Actions → Update profile visuals → Run workflow 手动触发，之后每天北京时间约 04:23 更新。使用 GitHub 自动提供的 GITHUB_TOKEN，无需手动添加密钥。仓库需允许 Actions 写入内容；分支保护规则可能阻止机器人直接推送。

本地贡献图目前为明确标注的等待画面，不是模拟贡献数据；工作流成功后会替换为 xiaozhaoben 的真实图像。本地未执行 GitHub Actions，发布后需确认首次运行结果。

远程图片直接引用，可用性受网络与第三方服务影响。插画及分隔线引用自参考项目，已在 README 底部注明来源；原作者仓库内容变动可能影响图片链接。彩蛋采用折叠交互，GitHub README 不运行任意 JavaScript。

# 红山文化申遗 · ICOMOS 评审预判与 OUV 策略工具

本仓库用于通过 GitHub Pages 托管单页研究工具网站（红山文化申遗 ICOMOS 评审预判与 OUV 策略）。

## 仓库内容

- `index.html` —— 网站全部内容（单文件，自包含，外部依赖仅为 Google Fonts CDN）
- `.nojekyll` —— 空文件，关闭 GitHub Pages 的 Jekyll 处理，保证原样发布

## 发布步骤（GitHub Pages）

1. 在 GitHub 新建仓库：登录 github.com → 右上角 "+" → "New repository"
   - 仓库名建议：`hongshan-ouv`（将决定网址后半段）
   - 设为 Public（GitHub Pages 免费版要求公开仓库）
   - 不勾选 "Add a README"（本包已含）
2. 上传文件：仓库页 → "Add file" → "Upload files" → 把本包的 `index.html`、`.nojekyll`、`README.md` 三个文件拖入 → 底部 "Commit changes"
   - （也可用 git 命令行：`git init && git add . && git commit -m "init" && git remote add origin git@github.com:<用户名>/hongshan-ouv.git && git push -u origin main`）
3. 开启 Pages：仓库 → Settings → 左侧 "Pages" → Source 选 "Deploy from a branch" → Branch 选 `main`、目录选 `/ (root)` → Save
4. 等 1–2 分钟，访问网址确认：
   - `https://<用户名>.github.io/hongshan-ouv/`
5. 确认无误后，把 PPT 中二维码指向的旧地址（https://hongshan-ouv.surge.sh）替换为新地址，重新生成二维码并更新 PPT。

## 可选：自定义域名

如已购买域名，在仓库根目录添加 `CNAME` 文件（内容为域名，如 `ouv.example.com`），并在域名服务商处添加 CNAME 记录指向 `<用户名>.github.io`。

## 当前线上版本

- 临时托管（surge.sh）：https://hongshan-ouv.surge.sh
  - 账号：hongshan-ouv-2026@outlook.com（未验证邮箱，临时使用）
  - 密码：Hs!2026ouv
  - 迁移到 GitHub Pages 后可弃用，或登录 surge.sh 自行管理。

# 第一次 PR 练习 · Practice Your First Pull Request

**EN:** A beginner-friendly repo: **edit one line**, open a **Pull Request**, get **automated checks** — merge when green (optional **auto-merge**).  
**中文：** 专为新手准备：只改一行、提 PR，**自动检查**通过后合并（可配置**自动合并**）。

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## Quick start · 三步上手

| Step | EN | 中文 |
|------|----|------|
| 1 | **Fork** this repository | **Fork** 本仓库 |
| 2 | In your fork, edit **`Contributors.md`**: add **one line** in the **middle** of the list (not first/last line) | 在 fork 里编辑 **`Contributors.md`**，在列表**中间**加**一行**（勿放在文件最上或最下） |
| 3 | Open a **Pull Request** to `main` | 向本仓库 **`main`** 提 **Pull Request** |

**Line format · 一行格式**（replace `YOUR_USERNAME` · 替换用户名）:

```markdown
- [YOUR_USERNAME](https://github.com/YOUR_USERNAME)
```

More detail: **[CONTRIBUTING.md](CONTRIBUTING.md)** · 详细步骤见贡献指南。

---

## Rules · 规则（CI will validate · 自动检查会校验）

| | EN | 中文 |
|---|----|------|
| ✅ | Only **`Contributors.md`** may change | 只允许改 **`Contributors.md`** |
| ✅ | **Exactly one line** added, format: `- [user](https://github.com/user)` | **只新增一行**，格式如上 |
| ✅ | Username: letters, numbers, `-` only | 用户名：字母、数字、连字符 `-` |
| ❌ | Do not edit others’ lines or other files | 勿改他人行或其它文件 |

After checks pass, the PR shows a green ✓. Maintainers may enable **auto-merge**.  
检查通过后 PR 显示绿色 ✓；维护者可开启**自动合并**。

---

## Local commands · 本地命令示例

```bash
# Clone YOUR fork · 克隆你的 fork（YOUR_USERNAME = your GitHub username）
git clone https://github.com/YOUR_USERNAME/first-pr-practice.git
cd first-pr-practice

git switch -c add-YOUR_USERNAME
# Edit Contributors.md — add your line in the middle · 在中间加一行后保存

git add Contributors.md
git commit -m "Add YOUR_USERNAME to contributors"
git push -u origin add-YOUR_USERNAME
```

Then on GitHub: **Compare & pull request** → target **`buyicoder/first-practice`** branch **`main`** (if you forked from it).  
然后在 GitHub 上从你的 fork 发起 PR，**base** 选上游仓库的 **`main`**。

---

## Stuck? · 遇到问题？

Open an Issue using the template **「第一次 PR 遇到问题」** / **First PR help**.  
使用 Issue 模板 **「第一次 PR 遇到问题」** 描述卡在哪一步。

---

## For maintainers · 维护者：自动合并

**EN:** Settings → General → **Allow auto-merge**; branch protection / rulesets: require status check **`validate`** (job from workflow **Validate PR**). On each PR: **Enable auto-merge** when checks pass.  
**中文：** 设置里开启 **Allow auto-merge**；分支规则要求检查 **`validate`** 通过。PR 页可 **Enable auto-merge**。细则见 [.github/AUTO_MERGE.md](.github/AUTO_MERGE.md)。

---

## License

MIT

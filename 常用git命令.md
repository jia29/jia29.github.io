好的 👍 我帮你把上面提到的 Git 命令整理分类，方便你以后查找和使用。

---

## 📂 一、仓库初始化与远程管理

```bash
# 初始化本地仓库
git init

# 添加远程仓库（origin 是别名，可以换）
git remote add origin https://github.com/你的用户名/仓库名.git

# 查看远程仓库地址
git remote -v

# 修改分支名为 main（兼容 GitHub 默认分支）
git branch -M main
```

---

## 📂 二、文件操作（提交）

```bash
# 添加所有文件到暂存区
git add .

# 提交文件
git commit -m "提交信息"

# 修改最近一次提交的作者信息（换邮箱时用）
git commit --amend --reset-author
```

---

## 📂 三、分支操作

```bash
# 查看本地分支
git branch

# 查看远程分支
git branch -r

# 查看本地 + 远程所有分支
git branch -a
```

---

## 📂 四、推送与拉取

```bash
# 推送到远程 main 分支（第一次加 -u 建立追踪关系）
git push -u origin main

# 以后直接推送
git push

# 强制推送（覆盖远程内容）
git push origin main --force

# 拉取远程 main 分支并合并
git pull origin main

# 拉取远程 main 分支并变基（避免多余的 merge 提交）
git pull origin main --rebase
```

---

## 📂 五、查看仓库内容

```bash
# 查看远程分支最新提交
git log origin/main --oneline

# 查看远程 main 分支最近 5 条提交
git log origin/main --oneline -5

# 查看当前仓库的文件（只读）
git checkout origin/main
```

---

## 📂 六、邮箱相关（解决 GH007 错误）

```bash
# 修改全局邮箱为 GitHub 提供的 noreply 邮箱
git config --global user.email "你的GitHub-noreply邮箱"

# 查看当前邮箱配置
git config user.email
```

---

⚡️你可以把这些整理到一个 **笔记或 cheat sheet** 里，随时复制粘贴。

要不要我帮你把这些命令做成一个「命令速查表（Markdown格式）」，你可以保存成 `.md` 文件，平时一打开就能快速查？
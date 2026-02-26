# 同步到 GitHub

本地已完成 `git init` 和首次提交。按下面步骤即可推到 GitHub。

## 1. 在 GitHub 上新建仓库

1. 打开 https://github.com/new  
2. **Repository name** 填：`AI-driven-CRISPR-github`（或你喜欢的名字）  
3. 选 **Public**，**不要**勾选 “Add a README”  
4. 点 **Create repository**

## 2. 在本地添加远程并推送

在项目目录下执行（把 `YOUR_USERNAME` 换成你的 GitHub 用户名）：

```bash
cd /yzx/Project/AI-driven-CRISPR-github

git remote add origin https://github.com/YOUR_USERNAME/AI-driven-CRISPR-github.git
git push -u origin main
```

若用 SSH：

```bash
git remote add origin git@github.com:YOUR_USERNAME/AI-driven-CRISPR-github.git
git push -u origin main
```

按提示登录或输入 token 即可完成推送。

## 3. 之后更新

改完文件后：

```bash
git add .
git commit -m "更新说明"
git push
```

---

**说明**：`综述初稿.md` 已加入 `.gitignore`，不会随仓库一起推送。

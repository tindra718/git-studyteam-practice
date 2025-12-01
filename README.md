# git-studyteam-practice
学习小组实践练习仓库
结合你小组 Git 练习仓库的场景，我为你整理了一份**结构化、易操作、带可复制代码块**的 `README.md` 模板，直接替换仓库信息就能使用，同时包含成员能快速上手的全流程指引：

```markdown
# git-studyteam-practice
学习小组 Git 协作实践练习仓库，通过本项目掌握 Fork、Clone、分支管理、PR 等完整 GitHub 协作流程～

## ⚠️ 前置准备
1. **安装 Git**：访问 [Git 官网](https://git-scm.com/) 下载对应系统版本，安装后打开终端（Windows 推荐 Git Bash），执行 `git --version` 验证是否安装成功。
2. **注册 GitHub 账号**：若未注册，访问 [GitHub 官网](https://github.com/) 完成注册并登录。

## 📝 完整操作步骤（按顺序执行）
### 1. Fork 本仓库
- 进入本仓库页面：`https://github.com/你的GitHub用户名/git-studyteam-practice`
- 点击页面右上角「Fork」按钮，选择自己的 GitHub 账号，等待仓库复制完成（Fork 后你将拥有仓库的个人副本）。

### 2. Clone 到本地
1. 进入你 Fork 后的仓库页面，点击「Code」按钮，复制 HTTPS/SSH 链接。
2. 打开终端，执行以下命令（替换为自己的仓库链接）：
```bash
# 克隆 Fork 后的仓库到本地
git clone https://github.com/你的用户名/git-studyteam-practice.git
# 进入项目目录
cd git-studyteam-practice
```

### 3. 创建个人分支
基于 `main` 分支创建专属分支（替换为自己的昵称/姓名），避免直接修改主分支：
```bash
# 新建并切换到个人分支
git checkout -b 你的昵称
# 示例：git checkout -b zhangsan
```

### 4. 添加学习笔记
1. 在仓库根目录创建以自己昵称命名的 Markdown 文件：
```bash
# Windows 系统
echo. > 你的昵称.md
# Mac/Linux 系统
touch 你的昵称.md
```
2. 打开文件，填写 Git 学习笔记（内容不限，建议包含学习心得、操作难点等），示例：
```markdown
# 张三的 Git 学习笔记
## 学习时间
2025-12-01

## 核心知识点
1. Fork 是复制仓库到自己的 GitHub 账号，不影响原仓库。
2. 分支可以隔离开发内容，避免主分支混乱。
3. PR 是向原仓库发起合并请求，需要仓库管理员审核。

## 遇到的问题
克隆仓库时输错了链接，后来重新复制 Fork 后的链接就解决了。
```

### 5. 提交更改并推送到远程
将本地修改提交并推送到你 Fork 后的远程仓库：
```bash
# 将文件添加到暂存区
git add 你的昵称.md
# 提交更改（备注清晰的提交信息）
git commit -m "Add 你的昵称.md: Git 学习笔记"
# 首次推送需关联远程分支，后续直接用 git push 即可
git push -u origin 你的昵称
```

### 6. 发起 Pull Request（PR）
1. 回到你 Fork 后的仓库页面，会看到「Compare & pull request」的提示按钮，点击进入。
2. 填写 PR 信息：
   - 标题：格式为 `Add 你的昵称's Git 学习笔记`（示例：`Add zhangsan's Git 学习笔记`）。
   - 描述：简单说明提交内容（如“提交个人 Git 学习笔记，完成协作流程练习”）。
3. 点击「Create pull request」，等待组长审核合并。

## 📌 规范要求
1. 分支命名：建议使用自己的昵称/姓名（如 `lisi`），禁止使用 `feature/xxx` 等格式。
2. 文件名：与分支名保持一致（如分支 `wangwu` 对应 `wangwu.md`），避免重复或格式错误。
3. 提交信息：需包含文件名，确保语义清晰，禁止无意义的“update”“fix”等备注。

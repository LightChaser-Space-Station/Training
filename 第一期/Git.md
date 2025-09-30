# 🌟 GitHub + VS Code 超级入门教程（小白友好·完整版）

---

## 一、什么是 GitHub？

* **简单理解**：GitHub = 「网盘 + 社区」

  * 你可以把代码/文件放上去，不怕丢失。
  * 别人也能看到、帮你修改，就像多人共享一个“电子笔记本”。

💡 GitHub 是全球最大的代码托管平台，很多大公司、大项目都在用。

---

## 二、开始使用 GitHub

### 1. 注册账号

1. 打开 [GitHub 官网](https://github.com/)。
2. 点击 **Sign up（注册）**。
3. 填写用户名、邮箱、密码。
4. 去邮箱收一封确认邮件 → 点击确认。📧

### 2. 创建仓库（相当于文件夹）

1. 登录 GitHub → 右上角点 **+ → New repository**。
2. 填一个名字（比如：`my-first-repo`）。
3. 勾选 **Add a README file**（加个说明文件）。
4. 点 **Create repository**。

🎉 这样，你就有了第一个 GitHub 仓库！

---

## 三、安装工具（CLI 方案更简单！）

### 1. 安装 VS Code

👉 [下载 VS Code](https://code.visualstudio.com/)
（这是一个强大的文本编辑器，用来写文件和操作源代码管理）。

### 2. 安装 GitHub CLI

👉 [下载 GitHub CLI](https://cli.github.com/)
（它内置 Git，不用单独装 Git，对新手更简单）。

### 3. 登录 GitHub CLI

打开终端，输入：

```bash
gh auth login
```

按提示选择：

* GitHub.com
* HTTPS
* Yes
* 输入 GitHub 用户名 & 密码

成功后，终端会显示 ✅ 登录成功。

---

## 四、操作流程（带图文流程图）

### 🔗 总流程（文字版）

```
[注册 GitHub] 
      │
      ▼
[创建仓库 (New repository)]
      │
      ▼
[安装 VS Code + GitHub CLI]
      │
      ▼
[gh auth login 登录]
      │
      ▼
[克隆仓库到本地]
   gh repo clone 用户名/仓库名
      │
      ▼
[用 VS Code 打开文件夹]
      │
      ▼
[修改文件 (README.md)]
      │
      ▼
[VS Code 源代码管理: 提交]
      │
      ▼
[推送到 GitHub → gh repo sync]
      │
      ▼
[完成 🎉]
```

---

### 🖼️ 图解步骤

#### 1. 注册 & 创建仓库

👉 登录 GitHub → 右上角 `+` → **New repository**

#### 2. 克隆到本地

在终端输入：

```bash
gh repo clone 用户名/仓库名
```

#### 3. 打开 VS Code

* 文件 → 打开文件夹 → 选中刚克隆的文件夹。

#### 4. 修改 & 提交

* 打开 `README.md`，写点内容。
* 左边点击 **源代码管理** → 输入备注（比如“第一次提交”）→ 点 ✅ 提交。

#### 5. 推送到 GitHub

```bash
gh repo sync
```

同步完成 → 你的修改就上 GitHub 啦！🚀

---

## 五、日常操作（最常用 3 步）

1. 改文件（写好内容）。
2. VS Code 源代码管理 → 提交。
3. `gh repo sync` → 推送到 GitHub。

---

## 六、分支（Branch）

> 可以先不管，理解成“不同版本的存档”。以后多人协作时才会用到。

---

## 七、遇到问题怎么办？

1. 推送失败？→ 检查网络 & 登录状态。
2. 出现冲突？→ VS Code 会标红，手动改掉，再提交。
3. 忘记命令？→ 用 VS Code 的按钮操作，也能完成大部分工作。

---

## 八、推荐插件（小白专用）

* **GitHub Pull Requests and Issues** → 在 VS Code 里直接操作 PR 和 Issues。
* **GitLens** → 显示是谁修改了代码、何时修改的。

---

## 九、练习任务（循序渐进）

1. 注册 GitHub。
2. 创建一个仓库。
3. 用 GitHub CLI 克隆到本地。
4. 在 VS Code 修改 `README.md`。
5. 提交并推送到 GitHub。

完成这 5 步，你就正式入门啦！🎉💯

---

# 使用说明
## 准备工作
1. 安装[Git](https://git-scm.com/)：版本控制系统（安装时勾选"Git Bash Here"）
2. 新建文件夹用于存放仓库文件。
## 初始化配置
### 打开`Git Bash`
```Git Bash
cd /e/code/Obsidian Vault/Team
```
解释：`e`是文件夹所在盘符，`Team`是新建文件夹名称
### 将Github仓库克隆到本地
```Git Bash
git clone https://github.com/weiyvshan/Team.git
```

### 创建自己的分支
```Git Bash
git checkout -b name
```
## 提交变更
### 添加所有更改
```Git Bash
git add .
```
### 添加描述
```Git Bash
git commit -m "添加示例"
```
### 推送到自己的分支
```Git Bash
git push origin name
```

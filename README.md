# 项目介绍
本项目是基于 Obsidian 构建的团队知识管理系统，采用 Git 版本控制实现多人协同编辑。通过结构化目录体系与 Git 分支策略，实现：

- **知识沉淀**：多领域知识的结构化存储与版本管理
- **智能检索**：支持双向链接、标签系统、全局搜索
- **协同创作**：多人协作编写技术文档、项目报告等
- **流程规范**：集成团队工作规范与协作模版
# 构建思路
## 技术架构
```mermaid                                                                  
graph TD    
    A[Git 版本控制] --> B(分支管理)
    A --> C(历史追溯)
    A --> D(冲突解决)
    E[Obsidian 核心] --> F(双向链接)
    E --> G(知识图谱)
    E --> H(模板系统)
```
## 协作方案
### 可视化文件树
```text
Team/
├── 00-团队规范/
|   ├── image/					#用于存放图片
│   ├── 常见问题及解决方案.md
│   └── 命名规则.md
├── 01-共享知识库/
│   ├── AI使用/
|   └── Obsidian插件推荐/
├── 02-学习笔记/
│   └── name/					#各自的学习成果
└── README.md
```
### 分支策略
- `main` 分支：稳定版本，仅包含审核通过的内容
- `name` 分支：成员个人工作分支
# 使用说明
![协作示意图](https://cdn.skyimg.de/up/2025/3/11/h1bgx2.webp)
## 准备工作
1. 安装[Git](https://git-scm.com/)：版本控制系统（安装时勾选"Git Bash Here"）
2. 新建文件夹，命名为`Team`用于存放仓库文件。
## 初始化配置
### 打开`Git Bash`
```Git Bash
cd "/e/code/Obsidian Vault/Team"
```
解释：`e`是文件夹所在盘符，`Team`是新建文件夹名称，`/e/code/Obsidian Vualt/Team`=`E:\code\Obsidian Vault\Team`是文件夹路径。（每个人路径不同，切勿直接复制）
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
## 合并分支
### 将分支的指定文件夹合并到主分支`main`
#### 1. 切换到主分支
```Git Bash
git checkout main
```
#### 2. 将分支`name`中指定文件夹的所有内容复制到当前分支
```Git Bash
git checkout name -- path/to/folder
```
#### 3. 接下来，使用`git add`命令将更改添加到暂存区。
```Git Bash
git add path/to/folder
```
#### 4. 提交合并结果
```Git Bash
git commit -m "Merge folder from branchA into main"
```
## 插件替代
[[01-共享知识库/Obsidian插件推荐/Obsidian-Git|Obsidian-Git]]
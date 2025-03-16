---
title: CherryStudio AI助手平台的使用
date: 2025-03-07T20:47:05.000Z
tags:
  - CherryStudio
  - 人工智能
categories:
  - 零基础入门
updated: '2025-03-07T15:26:28.131Z'
contentHash: 3c64ed52ef5bedf2f58920d8b70211aa
---

## CherryStudio

CherryStudio 是一款集多模型对话、知识库管理、AI 绘画、翻译等功能于一体的全能 AI 助手平台。

### 安装

1. 在[官网](https://cherry-ai.com)下载系统对应的客户端的安装包。
2. 打开安装包，选择为所有用户安装，更改安装目录（非C盘目录，降低系统卡顿）。

### 服务商配置

Cherry Studio通过AI服务商提供的api来实现与AI大模型的对话，因此我们首先要找到一个AI服务商

#### 服务商示例

##### 火山引擎（字节跳动）

1. 登录火山引擎，点击右上角控制台![image](https://cdn.skyimg.de/up/2025/3/7/phhvj6.webp)
2. 左方侧栏->系统管理->`API Key`管理![image](https://cdn.skyimg.de/up/2025/3/7/krwr5b.webp)创建`API Key`![image](https://cdn.skyimg.de/up/2025/3/7/o13ata.webp)
3. 左方侧栏->系统管理->开通管理 开通想要开通的模型服务，点击模型名进入详情页面![image](https://cdn.skyimg.de/up/2025/3/7/i4f05i.webp)记下`Model ID`
4. 回到Cherry Studio，右下角设置->模型服务->火山引擎 在API密钥中填入第二步得到的`API Key`![image](https://cdn.skyimg.de/up/2025/3/7/8iz1g1.webp)点击`添加`按钮在模型ID一栏填入第三步得到的`Model ID`![image](https://cdn.skyimg.de/up/2025/3/7/n820vv.webp)

### 对话界面

确保模型服务处于启用，到对话界面与AI对话。![image](https://cdn.skyimg.de/up/2025/3/7/lv2o6d.webp)

#### 助手

助手是对所选模型做一些个性化的设置来使用模型，如提示词预设和参数预设等，通过这些设置让所选模型能更加符合你预期的工作。

系统默认助手预设了一个比较通用的参数（无提示词），您可以直接使用或者到智能体页面寻找你需要的预设来使用。![image](https://cdn.skyimg.de/up/2025/3/7/68qlsq.webp)

##### 编辑助手

###### 名称

可自定义为方便辨识的助手名称。

###### 提示词

AI模型与你对话设定的身份，优秀的提示词能提高模型输出能力。  
例![image](https://cdn.skyimg.de/up/2025/3/7/04dmod.webp)

#### 话题

助手是话题的父集，单个助手下可以创建多个话题（即对话），所有话题共用助手的参数设置和预设词（prompt）等模型设置。![image](https://cdn.skyimg.de/up/2025/3/7/k1wdhu.webp)同个话题内，AI可根据上下文为你提供更符合的回答。

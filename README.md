# Blockly Games

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Deploy](https://img.shields.io/badge/Deploy-Cloudflare_Pages-F38020?logo=cloudflare&logoColor=white)](https://blockly-games.pages.dev)
[![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-222222?logo=github&logoColor=white)](https://github.com/mars-base/blockly-games)

Google 的可视化编程教育游戏，纯静态部署版本。

## 项目介绍

Blockly Games 是由 Google 开发的一系列教育游戏，旨在通过游戏化学习帮助初学者掌握编程基础概念。本项目将其构建为纯静态站点，可部署到 Cloudflare Pages、GitHub Pages 等任意静态托管平台。

## 包含的游戏

1. **Puzzle（拼图）** - Blockly 积木基础入门
2. **Maze（迷宫）** - 循环与条件语句
3. **Bird（鸟）** - 角度与坐标系统
4. **Music（音乐）** - 音乐创作与编程
5. **Turtle（海龟）** - 变量与函数
6. **Movie（电影）** - 动画制作
7. **Pond Duck（池塘鸭子）** - JavaScript 编程入门
8. **Pond Tutor（池塘导师）** - 高级 JavaScript 编程

## 特性

- ✅ 支持多语言（中文、英文等 60+ 种语言）
- ✅ 纯静态部署，无需后端服务器
- ✅ 支持 Cloudflare Pages、GitHub Pages 等静态托管平台
- ✅ 所有资源使用绝对路径，适配任意部署路径
- ✅ 内置"主页"导航按钮

## 构建要求

- Python 3.x
- Node.js（用于 Closure Compiler）
- Git

## 本地运行

```bash
cd blockly-games-deploy
python3 -m http.server 8080
```

访问 http://localhost:8080

## 部署到 Cloudflare Pages

1. Fork 本仓库到你的 GitHub 账号
2. 登录 Cloudflare Dashboard，进入 Pages
3. 创建新项目，连接 GitHub 仓库
4. 构建设置：
   - 生产分支：`main`
   - 根目录：`./`（仓库根目录）
   - 无需构建命令（直接部署静态文件）
5. 保存并部署

## 部署到 GitHub Pages

1. 进入仓库 Settings → Pages
2. Source 选择 "Deploy from a branch"
3. Branch 选择 `main`，目录选择 `/ (root)`
4. 保存后即可通过 `https://username.github.io/blockly-games` 访问

## 技术栈

- **前端框架**：Blockly（Google 的可视化编程库）
- **JavaScript 压缩**：Google Closure Compiler
- **构建工具**：Python 脚本
- **代码解释**：JS-Interpreter

## 许可证

Copyright 2012-2024 Google LLC

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

本项目基于 [Apache License 2.0](LICENSE) 开源。

## 致谢

感谢 Google 开发 Blockly Games 教育项目，让编程学习变得更加有趣和直观。

---

**演示站点**：https://blockly-games.pages.dev

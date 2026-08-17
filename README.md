<h1 align="center">DPanel 第三方应用商店</h1>

<p align="center">
  适配 <code>DPanel</code> 应用商店 的 Docker 应用配置合集。可直接在DPanel中导入应用商店。
</p>

<p align="center">
  <img src="docs/afdian-logo.png" alt="Docker Apps 项目标识" width="640">
</p>

<p align="center">
  <a href="README.md"><img src="https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-2875B6?style=flat-square" alt="简体中文（当前语言）"></a>
  <a href="README-en.md"><img src="https://img.shields.io/badge/English-D9D9D9?style=flat-square" alt="Read in English"></a>
</p>

## 支持项目

<p align="center">
  <a href="https://ifdian.net/a/QUAN_GE"><strong>爱发电赞助：用爱发电</strong></a><br><br>
</p>

<details>
<summary><strong>目录</strong></summary>

- [支持项目](#支持项目)
- [免责声明](#免责声明)
  - [1. 镜像容器适配](#1-镜像容器适配)
  - [2. 法律遵守](#2-法律遵守)
  - [3. 免责声明接受](#3-免责声明接受)
- [1. 简介](#1-简介)
- [2. 使用方式](#2-使用方式)
- [3. 贡献应用](#3-贡献应用)
- [已下架应用](#已下架应用)

</details>

***

## 免责声明

### 1. 镜像容器适配

本项目仅针对原`docker`镜像容器运行进行针对`1Panel`应用商店的适配。我们不对任何原始镜像的有效性做出任何明示或暗示的保证或声明，并且不对使用本仓库应用所造成的任何影响负责。用户在使用本项目时应自行承担风险。

### 2. 法律遵守

用户在使用本仓库时必须遵守所在国家与地区的法律法规。某些应用可能受到特定国家法律的限制，用户需自行了解并遵守相关法律要求。本仓库不对用户违反法律法规所产生的任何后果负责。

### 3. 免责声明接受

用户在导入本仓库并使用其中的应用时，即表示用户已经阅读、理解并同意接受本免责声明的所有条款和条件。

请注意，本免责声明仅针对本仓库的使用情况，并不包括其他第三方应用或服务。对于与本仓库链接的第三方内容，我们不对其准确性、完整性、可靠性或合法性负责。

在使用本仓库之前，请确保已经阅读、理解并接受了本免责声明的所有条款和条件。

***

## 1. 简介

本仓库按 1Panel v2 应用规范组织应用目录、元数据、表单变量和 Docker Compose 配置，尽量做到导入后即可安装，减少手动部署和重复配置。

## 2. 使用方式

面板中添加自定义应用商店：

    https://github.com/quan-ge/dpanel-appstore

国内网络不佳请使用：

    https://down.nigx.cn/github.com/quan-ge/dpanel-appstore

## 3. 贡献应用

> [!IMPORTANT]
> 第三方开发者提交应用 PR 前，建议先使用 [okxlin/1panel-app-adapter](https://github.com/okxlin/1panel-app-adapter) 生成或校验应用包。它会检查 1Panel v2 目录结构、`data.yml`、`docker-compose.yml`、环境变量闭包、i18n 标签和常见发布问题，能减少返工。

提交 PR 时请优先提供可复现的官方来源、镜像来源、默认端口、数据目录、前置依赖和测试结果。仓库只需要最终应用目录，不需要提交临时测试产物或过程文件。

## 已下架应用

无法安装且没有可信替代镜像的应用会从活动目录移除，避免继续展示给新用户。下架原因和最后版本记录在 [`.github/retired-apps.yml`](.github/retired-apps.yml)，完整应用文件仍可从 Git 历史恢复。
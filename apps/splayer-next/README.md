<div align="center">
<img alt="logo" height="100" width="100" src="https://github.com/SPlayer-Dev/SPlayer/blob/dev/public/icons/favicon.png?raw=true" />
<h2> SPlayer </h2>
<p> 一个简约的音乐播放器 </p>

[API Docs](https://splayer.imsyy.top/api.html) | [开发版](https://github.com/imsyy/SPlayer/actions) | [发行版](https://splayer.imsyy.top/download.html)

<br />

[![Stars](https://img.shields.io/github/stars/imsyy/SPlayer?style=flat)](https://github.com/imsyy/SPlayer/stargazers)
[![Version](https://img.shields.io/github/v/release/imsyy/SPlayer)](https://github.com/imsyy/SPlayer/releases)
[![Build Release](https://github.com/imsyy/SPlayer/actions/workflows/release.yml/badge.svg)](https://github.com/imsyy/SPlayer/actions/workflows/release.yml)
[![License](https://img.shields.io/github/license/imsyy/SPlayer)](https://github.com/imsyy/SPlayer/blob/dev/LICENSE)
[![Issues](https://img.shields.io/github/issues/imsyy/SPlayer)](https://github.com/imsyy/SPlayer/issues)
[![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/imsyy/SPlayer)

</div>

![main](https://github.com/SPlayer-Dev/SPlayer/blob/dev//screenshots/SPlayer.jpg?raw=true)

## 说明


> [!CAUTION]
>
> # 本项目进入维护模式
>
> 项目已进入维护模式，后续仅进行必要的维护与重大问题修复，不再主动开发新功能
>


- 本项目采用 [Vue 3](https://cn.vuejs.org/) + [TypeScript](https://www.typescriptlang.org/) + [Naïve UI](https://www.naiveui.com/) + [Electron](https://www.electronjs.org/zh/docs/latest/) 开发
- Node.js 版本要求：>= 20，包管理器：pnpm >= 10
- 默认会构建原生模块，需准备 Rust 工具链；如仅需要网页端构建或暂时跳过，可设置环境变量 `SKIP_NATIVE_BUILD=true`
- 支持网页端与客户端，由于设备有限，目前仅保证 Windows 系统的适配，其他平台如遇问题可以提 Issue 或自行解决后选择提 PR
- 欢迎各位大佬 `Star` 😍


## 🧑‍💻 开发

### 快速开始

1. 安装依赖：`pnpm install`
2. 复制 `.env.example` 为 `.env` 并按需修改
3. 启动开发：`pnpm dev`
4. 构建：
   - `pnpm build`
   - `pnpm build:win`

### 跳过原生模块构建

默认会编译 `native/*` 下的原生模块（需要 Rust）。如果你的场景不需要原生能力，可设置 `SKIP_NATIVE_BUILD=true` 后再执行 `pnpm dev` / `pnpm build`。


## 🎉 功能

- ✨ 支持扫码登录
- 📱 支持手机号登录
- ~~📅 自动进行每日签到及云贝签到~~
- 💻 支持桌面歌词
- 💻 支持切换为本地播放器，此模式将不会连接网络
- 🎨 封面主题色自适应，支持全站着色
- 🌚 Light / Dark / Auto 模式自动切换
- 📁 本地歌曲管理及分类（建议先使用 [音乐标签](https://www.cnblogs.com/vinlxc/p/11347744.html) 进行匹配后再使用）
- 📁 本地音乐标签编辑及封面修改
- ➕ 新建歌单及歌单编辑
- ❤️ 收藏 / 取消收藏歌单或歌手
- ☁️ 云盘音乐上传
- 📂 云盘内歌曲播放
- 🔄 云盘内歌曲纠正
- 🗑️ 云盘歌曲删除
- 🌐 支持 Subsonic / Navidrome 等流媒体服务（多服务器支持、自动连接）
- 📝 支持逐字歌词
- 🔄 歌词滚动以及歌词翻译
- 📹 MV 与视频播放
- 🎶 音乐频谱显示
- ⏭️ 音乐渐入渐出
- 🔄 支持 PWA
- 💬 支持评论区
- 🎵 支持 Last.fm Scrobble（播放记录上报）
- 📱 移动端基础适配

## 🖼️ 界面展示

<details>
<summary> 主页面 </summary>

![主页面](https://github.com/SPlayer-Dev/SPlayer/blob/dev//screenshots/SPlayer%20-%20主页面.jpg?raw=true)

</details>

<details>
<summary> 播放页面 </summary>

![播放页面](https://github.com/SPlayer-Dev/SPlayer/blob/dev//screenshots/SPlayer%20-%20播放页面.jpg?raw=true)

</details>

<details>
<summary> 发现页面 </summary>

![发现页面](https://github.com/SPlayer-Dev/SPlayer/blob/dev//screenshots/SPlayer%20-%20发现页面.jpg?raw=true)

</details>

<details>
<summary> 歌单页面 </summary>

![发现页面](https://github.com/SPlayer-Dev/SPlayer/blob/dev//screenshots/SPlayer%20-%20歌单页面.jpg?raw=true)

</details>

<details>
<summary> 评论页面 </summary>

![发现页面](https://github.com/SPlayer-Dev/SPlayer/blob/dev//screenshots/SPlayer%20-%20评论页面.jpg?raw=true)

</details>

<details>
<summary> 本地音乐 </summary>

![发现页面](https://github.com/SPlayer-Dev/SPlayer/blob/dev//screenshots/SPlayer%20-%20本地音乐.jpg?raw=true)

</details>


## 😘 鸣谢

特此感谢为本项目提供支持与灵感的项目：

- [NeteaseCloudMusicApi](https://github.com/neteasecloudmusicapienhanced/api-enhanced)
- [YesPlayMusic](https://github.com/qier222/YesPlayMusic)
- [UnblockNeteaseMusic](https://github.com/UnblockNeteaseMusic/server)
- [applemusic-like-lyrics](https://github.com/Steve-xmh/applemusic-like-lyrics)
- [Vue-mmPlayer](https://github.com/maomao1996/Vue-mmPlayer)
- [refined-now-playing-netease](https://github.com/solstice23/refined-now-playing-netease)
- [material-color-utilities](https://github.com/material-foundation/material-color-utilities)



## 📢 免责声明

本项目部分功能使用了网易云音乐的第三方 API 服务，**仅供个人学习研究使用，禁止用于商业及非法用途**

同时，本项目开发者承诺 **严格遵守相关法律法规和网易云音乐 API 使用协议，不会利用本项目进行任何违法活动。** 如因使用本项目而引起的任何纠纷或责任，均由使用者自行承担。**本项目开发者不承担任何因使用本项目而导致的任何直接或间接责任，并保留追究使用者违法行为的权利**

请使用者在使用本项目时遵守相关法律法规，**不要将本项目用于任何商业及非法用途。如有违反，一切后果由使用者自负。** 同时，使用者应该自行承担因使用本项目而带来的风险和责任。本项目开发者不对本项目所提供的服务和内容做出任何保证

感谢您的理解


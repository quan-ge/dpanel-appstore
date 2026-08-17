
<div style="border: 1px solid #FFC107; padding: 10px; border-radius: 5px; color: #856404; background-color: #FFF3CD; display: inline-block; width: 100%; max-width: 60%; margin-top: 10px;">
    <div style="display: flex; align-items: center;">
        <span style="font-size: 24px; margin-right: 8px;">⚠️</span>
        <div>
            <strong style="font-size: 16px;">温馨提示</strong><br>
            <span style="font-size: 14px; color: #333;">启动后访问：<code>http://127.0.0.1:9090/ui/</code></span><br />
            <span style="font-size: 14px; color: #333;">首次访问需要配置：</span><br />
            <span style="font-size: 14px; color: #333;">- 后端地址：<code>http://127.0.0.1:9090</code><br />
            <span style="font-size: 14px; color: #333;">- 密钥：与你填写 一致 </span><br />
        </div>
    </div>
</div>

# Clash for Docker
![GitHub Repo stars](https://img.shields.io/github/stars/gangz1o/clash4docker?style=for-the-badge)
![GitHub forks](https://img.shields.io/github/forks/gangz1o/clash4docker?style=for-the-badge)
![GitHub contributors](https://img.shields.io/github/contributors/gangz1o/clash4docker?style=for-the-badge)
![GitHub repo size](https://img.shields.io/github/repo-size/gangz1o/clash4docker?style=for-the-badge)
![GitHub issues](https://img.shields.io/github/issues/gangz1o/clash4docker?style=for-the-badge)
![Docker Pulls](https://img.shields.io/docker/pulls/gangz1o/glash?style=for-the-badge)

🚀 基于最新 **Mihomo** 内核，内置 Dashboard 的 Clash Docker 镜像


# <h1 style="font-size:34px;font-weight:700;background:linear-gradient(135deg,#3b82f6,#8b5cf6);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;padding:8px 0;">界面一览</h1>
<details>
  <summary style="cursor:pointer;font-size:24px;">点击展开</summary>
    <img src="https://cdn.nodeimage.com/i/5Q9E9uQk9j6x9tkCSMu9MDxY56MYklUg.webp" alt="Image 1">
    <img src="https://cdn.nodeimage.com/i/kWcCiiHfK3fmyFWQaC6Ndkh0vnfLj0lP.webp" alt="Image 2">
    <img src="https://cdn.nodeimage.com/i/vA3jgJCQmhsLNVqoNWj8cKvqovJmX4QK.webp" alt="Image 3">
    <img src="https://cdn.nodeimage.com/i/zDENCwikV4ZKAxrBwPjKsj3MXUYTpxiR.webp" alt="Image 4">
    <img src="https://cdn.nodeimage.com/i/zDENCwikV4ZKAxrBwPjKsj3MXUYTpxiR.webp" alt="Image 5">
    <img src="https://cdn.nodeimage.com/i/gvdOcbUtUASmKtlfKY7crcokkIQYY0nM.webp" alt="Image 6">
</details>


## 核心特性

- ✅ Mihomo (Clash Meta)最新内核
- ✅ MetacubexD Web Dashboard 内置
- ✅ 预打包 GeoIP 数据库，无需运行时下载
- ✅ 支持 amd64 / arm64 架构
- ✅ **订阅功能**：支持远程订阅链接自动下载配置
- ✅ **自动更新**：支持定时自动更新订阅并重启生效
- ✅ **容错处理**：订阅下载失败时自动回退到本地配置

## 支持的协议（可能列的不全，以mihomo支持的协议为主）

| 协议             | 说明                      |
| ---------------- | ------------------------- |
| Shadowsocks (SS) | 经典轻量级加密代理        |
| VMess            | V2Ray 原生协议            |
| VLESS            | V2Ray 轻量协议，性能更优  |
| Trojan           | 基于 TLS 的隐蔽协议       |
| Hysteria         | 基于 QUIC 的高速协议      |
| Hysteria2        | Hysteria 第二代，更快更稳 |
| TUIC             | 基于 QUIC 的多路复用协议  |
| WireGuard        | 现代化 VPN 协议           |
| HTTP             | HTTP/HTTPS 代理           |
| SOCKS5           | 通用 SOCKS5 代理          |



### 环境变量

| 变量               | 说明                                                           | 示例                      |
| ------------------ | -------------------------------------------------------------- | ------------------------- |
| `SUB_URL`          | 订阅地址，支持返回 Clash 配置的链接                            | `https://example.com/sub` |
| `SUB_CRON`         | 自动更新的 cron 表达式                                         | `0 */6 * * *`             |
| `SECRET`           | Dashboard 登录密钥，会自动注入配置                             | `my-password`             |
| `ALLOW_LAN`        | 是否允许局域网连接，默认不修改配置                             | `true` 或 `false`         |
| `TUN_ENABLED`      | 是否启用 TUN 模式，重启后自动恢复（需配合 Docker 权限）        | `true` 或 `false`         |
| `DOWNLOAD_PROXY`   | 首次下载订阅时使用的外部代理（可选）                           | `http://192.168.1.1:7890` |
| `SUB_USER_AGENT`   | 下载订阅时使用的 User-Agent，默认 `clash.meta`（可选）         | `clash.meta`              |
| `DNS_OVERRIDE`     | DNS复写功能，此功能仅针对不含DNS规则内容的Clash订阅链接（可选）                 | `true` 或 `false`         |
| `AUTHENTICATION`   | HTTP 基本认证凭据，格式 `username:password`，自动注入配置文件（可选） | `user:pass`               |


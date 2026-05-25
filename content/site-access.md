---
title: "如何访问本站"
description: "本地预览与线上访问方式说明。"
---

## 本地访问（推荐）

1. 安装 Hugo（extended 版本）。
2. 在仓库根目录执行：

```bash
hugo server -D --bind 0.0.0.0 --port 1313
```

3. 在浏览器打开：

- `http://localhost:1313/`

如果你在远程开发环境（如容器/云 IDE），需要使用平台提供的 **Port 1313 转发地址** 打开页面。

## 线上访问

当前 `hugo.yaml` 的 `baseURL` 配置为：

- `https://wuming9.github.io/pkydrip-docs/`

部署完成后可直接访问该地址。

## 常见问题

- 提示 `hugo: command not found`：说明本机未安装 Hugo，需要先安装后再运行本地预览命令。
- 页面为空或样式异常：确认你是在仓库根目录执行命令，并且访问的是 `1313` 端口。

- 页面空白：通常是部署目录配置错误（应发布 Hugo 生成目录，如 `public/`），或域名/CDN 仍指向旧站点。

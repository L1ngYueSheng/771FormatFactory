# 771 Format Factory（独立版）

从 **柒柒壹工具箱** 里单独拆出来的格式转换工具：**一个入口 exe，双击即用**，不依赖工具箱、也不用安装任何东西。
注:该软件为100%AI

当前版本：**v2.0.5**（2026-10-16）· Windows 10 / 11（64 位）

> **v2.0 起软件换成 Flutter 新版外壳**——同一个软件、同一个入口 exe 名称，使用习惯不变；
> **ffmpeg 引擎已打进安装包**，换台没装过 ffmpeg 的电脑也能直接转。
> 旧版（v1.12，tkinter 外壳）仍可在历史 Release 下载；旧版的音乐解密、PDF 深化等少数功能
> 尚未在新外壳里提供，如你依赖这些功能可继续用旧版。

**带联网自动更新**：启动后后台查新（失败静默），发现新版弹窗询问，下载后自动校验
（Ed25519 签名 + SHA-256）再替换并重启。

## 功能（自带 ffmpeg 引擎）
- 文档：md / html / txt / csv 互转
- 图片：jpg / png / webp / bmp 互转；按宽度等比缩放
- 数据：json / yaml / csv / xml 互转；配置：json / env / ini 互转
- PDF：图片 → 单页 PDF
- 音视频：mp3 / m4a / wav / mp4 / gif（内置 ffmpeg）
- 目标重名自动加序号，绝不覆盖已存在文件；队列日志逐条显示

## 下载
到 [Releases](../../releases/latest) 下载最新 zip，解压双击 `771FormatFactory.exe` 即用。

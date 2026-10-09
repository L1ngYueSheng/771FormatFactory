# 771 Format Factory（独立版）

从 **柒柒壹工具箱** 里单独拆出来的格式转换工具：**只有一个 exe，双击即用**，不依赖工具箱、也不用安装任何东西。
注:该软件为100%AI

文档 / 图片 / 音视频 / 数据配置 四类格式互转，另可读加密音乐文件（网易云 .ncm、酷狗 .kgm/.kgma/.vpr、QQ .qmc*/.mflac/.mgg），
还有 PDF 合并拆分提取、图片批量压缩 / 改尺寸 / 加水印。

当前版本：**v1.7**（2026-10-09）· Windows 10 / 11（64 位）

**从 v1.7 起带联网自动更新**：启动后后台查一次新版本（失败静默），有新版才弹窗问你要不要更新，
下载后自动校验（Ed25519 签名 + SHA-256）再替换并重启。也可以手动到 Releases 下载。

> 2026-10-09 起本工具与仓库名对齐：原「柒柒壹格式转换工具」→ **771 Format Factory**，exe 文件名 `771FormatFactory.exe`。

## 下载

到 [Releases](https://github.com/L1ngYueSheng/771FormatFactory/releases) 页面：

| 文件 | 说明 |
| --- | --- |
| `771FormatFactory.exe` | 单文件，双击即用（约 68 MB —— 大头是内置的 ffmpeg） |
| `771FormatFactory_v1.7.zip` | 上面那个 exe + 使用说明 |

> 资产名只能是 ASCII（GitHub 会把非 ASCII 字符剥掉），所以这里叫 `771FormatFactory.exe`。

## 能转什么

- **文档**：docx / pdf / txt / md / html 等互转（docx、pypdf、reportlab）。
- **图片**：jpg / png / webp / bmp / tiff / gif / ico / avif 等互转；另有「图片工具」页做批量压缩（按质量或目标体积上限）、改尺寸、加水印。
- **音视频**：内置 ffmpeg（essentials 构建）负责转码与音轨提取（mp3 / mp2 / aac / wav / flac 等目标）。
- **数据配置**：json / yaml / csv / xlsx 等互转。
- **加密音乐解密**：网易云 .ncm、酷狗 .kgm/.kgma/.vpr、QQ 音乐 .qmc*/.mflac/.mgg（自带密钥的版本），**只在本地解密**。
- **PDF 工具 / 图片工具**（增强页）：合并、按页拆分、提取指定页；批量压缩、改尺寸、文字/图片水印。
- 支持把文件**直接拖进窗口**；转换日志在窗口下方，出问题能看到具体原因。

> 除了「查更新」那一处（只读 GitHub Releases 的清单，失败静默），本程序**不联网**。

## 最近几版

- **v1.7** 加**联网自动更新**（与工具箱、截图工具同一套：Ed25519 验签清单 + SHA-256 校验 + 助手替换重启）；与仓库名对齐改名 771 Format Factory。
- **v1.6** 与主程序同源：接线 转换增强.py（PDF 工具 / 图片工具两页）。
- **v1.5** 与工具箱 v1.10 同源：阶段二转换类四项（PDF / 图片 / 正则改名 / 拖拽解压 + 加密压缩）。

## 相关

完整版（格式转换 / 批量改名 / 视频下载 / 压缩解压 / 截图 五合一）：<https://github.com/L1ngYueSheng/771Toolbox>

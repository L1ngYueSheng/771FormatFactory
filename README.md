# 771 Format Factory（独立版）

从 **柒柒壹工具箱** 里单独拆出来的格式转换工具：**一个入口 exe，双击即用**，不依赖工具箱、也不用安装任何东西。
注:该软件为100%AI

当前版本：**v2.0.21**（2026-11-11）· Windows 10 / 11（64 位）

- **主题切换闪烁与更新器修复（v2.0.21）**：主题涟漪第二次切换前先 stop 并归零，不再先露新主题一帧；补原生标题栏跟随深浅色；更新器流式下载/解压、验签移 Isolate、更新助手 /MIR+失败提示、staging 标记、体积上限、直连路线、检查可取消；OCR 临时文件唯一、单实例不静默退出；ffmpeg stderr 只对错误加 ⚠、ffmpeg 路径先查 PATH；状态栏动态系统版本。
## 免责声明

- 本软件仅供个人学习、研究与合法用途，请遵守当地法律法规及所用平台的服务条款。
- 请勿使用本软件侵犯他人知识产权、绕过付费/权限/地区限制，或制作、传播违法内容。
- 软件按“现状”提供，不保证无错误或不中断；因使用本软件产生的任何直接或间接后果由使用者自行承担。
- 第三方组件（如 ffmpeg / yt-dlp / 7z 等）归其各自作者所有，遵循各自许可证。


> **v2.0 起软件换成 Flutter 新版外壳**——同一个软件、同一个入口 exe 名称，使用习惯不变；
> **ffmpeg 引擎已打进安装包**，换台没装过 ffmpeg 的电脑也能直接转。
> 旧版（v1.12，tkinter 外壳）仍可在历史 Release 下载。

**带联网自动更新**：启动后后台查新（失败静默），发现新版弹窗询问，下载后自动校验
（Ed25519 签名 + SHA-256）再替换并重启。

## 批量转换（v2.0.19）

格式转换页可在 **单文件 / 批量** 之间切换。批量模式支持：

- 「添加文件…」多选（Windows 原生多选对话框）；
- 「添加文件夹…」按当前类别的扩展名扫描顶层文件；
- 也可以直接在文本框里每行贴一个路径；
- 逐文件日志 + 最终汇总（成功 / 失败 / 跳过），单个失败不中断；
- 输出重名自动加 `(1)`、`(2)`，不覆盖已有文件；
- 转换中可点「取消」，当前文件完成后停止。

单文件模式与原来的流程完全一致。

## PDF 转换（v2.0.20）

格式转换 → PDF 工具 下新增：

- **PDF 转 Word / Excel / PPT / TXT**（文字提取版，不保留原排版）；
- **PDF 逐页转图片**（DPI 96 / 150 / 200 / 300，存到「_逐页图片」文件夹）；
- **PDF 转长图**（全部页纵向拼接成一张 PNG）；
- **Office 转 PDF**（Word / Excel / PPT / ODF 等，需要本机安装 LibreOffice）。

PDF 文本提取与逐页渲染使用随包 Xpdf 工具（GPL，许可证在 `引擎/pdf`）；Office 相关转换需要本机安装 LibreOffice（免费）。


## 功能（自带 ffmpeg 引擎）
- **界面与主题（v2.0.18）**：浅色 / 深色 / 跟随系统；切换时从「主题」控件中心向外扩张成水滴涟漪（400 ms），圆边缘带一条淡出的高光细环
- **字幕**：SRT / ASS / SSA / VTT 互转；把字幕以 mov_text 字幕轨嵌入 MP4；非 UTF-8 字幕会提示先转存
- **视频 / 音频**：mp4 / mkv / avi / mov / webm / ts / mp3 / flac / wav / m4a / aac / ogg / opus 等常见格式互转；
  H.265 / AV1 / ProRes / FFV1 / HLS 切片 / DVD VOB / AMR-WB；
- **视频压缩（v2.0.17 新增）**：目标体积两遍编码 / CRF 质量档 / 1080p·720p·480p / 实时进度可取消
  SWF / RM / WTV / IVF / PSP / VCD / SVCD / SMJPEG / Huffyuv / Ut Video / MagicYUV / libx264rgb 等兼容用途格式
- **无损与特殊音频**：ALAC / WavPack / TTA / FLAC；aptX / aptX HD / Speex / GSM /
  G.711 A-law·μ-law / G.722 / G.723.1 / G.726 / W64 / MMF / IRCAM / SoX / AST / ADX / SBC
- **图片 34 种**：jpg / png / webp / bmp / gif / tiff / ico / tga / qoi / jp2 / ppm / pcx / sgi / xbm，
  以及 EXR / HDR / DPX / FITS / PAM / PBM / PGM / PFM / PHM / PGMYUV / WBMP / XWD /
  Sun Raster / JPEG-LS / ljpeg / Alias PIX / XFace；AVIF / APNG / 动图 WebP
- **图像序列**：视频导出 PNG / JPG 序列；图片序列合成视频（序号断档会明确报错）
- **文档 / 数据 / 配置**：md / html / txt / csv / docx / rtf；json / yaml / csv / xml / toml / properties；json / env / ini
- **PDF 与图片工具**：图片 → 单页 PDF；按宽度等比缩放
- **加密音乐解密**：ncm / kgm / kgma / vpr / qmc / mflac / mgg
- “转成格式”下拉框可搜索，只搜当前类别；目标重名自动加序号，绝不覆盖已存在文件；队列日志逐条显示

## 下载
到 [Releases](../../releases/latest) 下载最新 zip，解压双击 `771FormatFactory.exe` 即用。

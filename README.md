# 771 Format Factory（独立版）

从 **柒柒壹工具箱** 里单独拆出来的格式转换工具：**一个入口 exe，双击即用**，不依赖工具箱、也不用安装任何东西。
注:该软件为100%AI

当前版本：**v2.0.17**（2026-10-21）· Windows 10 / 11（64 位）

> **v2.0 起软件换成 Flutter 新版外壳**——同一个软件、同一个入口 exe 名称，使用习惯不变；
> **ffmpeg 引擎已打进安装包**，换台没装过 ffmpeg 的电脑也能直接转。
> 旧版（v1.12，tkinter 外壳）仍可在历史 Release 下载。

**带联网自动更新**：启动后后台查新（失败静默），发现新版弹窗询问，下载后自动校验
（Ed25519 签名 + SHA-256）再替换并重启。

## 功能（自带 ffmpeg 引擎）
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

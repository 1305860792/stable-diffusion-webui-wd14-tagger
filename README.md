&lt;!--
Stable Diffusion WebUI 中文安装指南

&gt; 基于 AUTOMATIC1111/stable-diffusion-webui 官方文档的社区中文翻译。  
&gt; 若需英文原版请移步 [官方 Wiki](https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki)。

---

硬件支持一览
| 平台 | 说明 | 外部文档 |
|---|---|---|
| NVIDIA GPU | 官方主力支持，CUDA 加速 | [Wiki](https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/Install-and-Run-on-NVidia-GPUs) |
| AMD GPU | 需 ROCm 驱动 | [Wiki](https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/Install-and-Run-on-AMD-GPUs) |
| Intel Arc / UHD / Iris | 社区实验性支持 | [外部 Wiki](https://github.com/openvinotoolkit/stable-diffusion-webui/wiki) |
| Intel CPU | 纯 CPU 推理，速度较慢 | 本文档 |
| 昇腾 NPU | 华为 Atlas 200/300 | [外部 Wiki](https://gitee.com/ascend/StableDiffusion) |

---

在线服务（免安装）
没有显卡或只想尝鲜？可直接使用 Colab 等在线服务：  
👉 [在线服务列表（官方维护）](https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/Online-Services)

---

Windows 安装

Release 包一键启动（NVIDIA 推荐）
1. 下载 [sd.webui.zip (v1.0.0-pre+)](https://github.com/AUTOMATIC1111/stable-diffusion-webui/releases) 并解压到任意目录。  
2. 双击 `update.bat` → 自动拉取最新代码。  
3. 双击 `run.bat` → 浏览器自动打开 `http://127.0.0.1:7860`。  
&gt; 详细参数调整见同目录 `webui-user.bat`。

全自动安装（含 AMD / Intel）
1. 安装 Python 3.10.6（更高版本会导致 torch 不兼容）  
   勾选 “Add Python to PATH”。  
   下载地址：https://www.python.org/ftp/python/3.10.6/python-3.10.6-amd64.exe  
2. 安装 [Git for Windows](https://git-scm.com/download/win)。  
3. 打开 PowerShell / CMD，克隆仓库：
   ```bat
   git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui.git
   cd stable-diffusion-webui

完成后在拓展插件页面安装stable-diffusion-webui-wd14-tagger（通过网址下载https://github.com/picobyte/stable-diffusion-webui-wd14-tagger）
然后点击应用并重启用户页面即可运行

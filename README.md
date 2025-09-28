# stable-diffusion-webui-wd14-tagger
项目实训作业
安装与运行
请确保满足所需依赖，并参考以下对应平台的说明：
NVIDIA 显卡（推荐）
AMD 显卡
Intel CPU、Intel 核显及独显
也可直接选用在线服务（如 Google Colab）：
Windows 10/11 + NVIDIA 显卡 快速安装（用发布包）
下载 sd.webui.zip 并解压。
双击 update.bat 更新。
双击 run.bat 启动。
更详细说明见 Install-and-Run-on-NVidia-GPUs。
Windows 全自动安装
安装 Python 3.10.6（更高版本不兼容 PyTorch），勾选 “Add Python to PATH”。
安装 Git。
克隆仓库：
git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui.git
进入解压后的文件夹，普通用户身份 双击 webui-user.bat，等待自动完成。
Linux 全自动安装
安装依赖（任选对应发行版命令）：
Debian/Ubuntu：
bash
sudo apt update
sudo apt install -y wget git python3 python3-venv libgl1 libglib2.0-0
Red Hat/CentOS/Fedora：
bash
sudo dnf install -y wget git python3 gperftools-libs libglvnd-glx
openSUSE：
bash
sudo zypper install -y wget git python3 libtcmalloc4 libglvnd
Arch/Manjaro：
bash
sudo pacman -S wget git python3
若系统默认 Python 版本过高（≥3.12），需手动装 3.10/3.11 并指定：
Ubuntu 24.04 示例：
bash
sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt update
sudo apt install python3.11
Arch 示例：
bash
sudo pacman -S yay
yay -S python311
然后在启动脚本里指定：
bash
export python_cmd="python3.11"
# 或编辑 webui-user.sh 加入：
python_cmd="python3.11"
下载并运行一键脚本：
bash
# 方法 1：直接拉脚本
wget -q https://raw.githubusercontent.com/AUTOMATIC1111/stable-diffusion-webui/master/webui.sh
chmod +x webui.sh
./webui.sh
# 方法 2：先克隆仓库
git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui.git
cd stable-diffusion-webui
./webui.sh
需要调参时编辑 webui-user.sh

完成后在拓展插件页面安装stable-diffusion-webui-wd14-tagger（通过网址下载https://github.com/picobyte/stable-diffusion-webui-wd14-tagger）
然后点击应用并重启用户页面即可运行

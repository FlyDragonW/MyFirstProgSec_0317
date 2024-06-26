# MyFirstProgramSec_0317
- 本課程屬於初階的入門課程
- 課程主要內容在簡報，此處主要是放指令和程式碼方便複製  

## 課前準備
- 練習虛擬機使用和 Linux 基本指令
- 安裝所需工具或使用我提供的虛擬機檔案

## 環境
虛擬機檔案載點：[分流1](https://drive.google.com/file/d/1hRD0UoNMt8flW2SJuIZf5L5QojCcTlm-/view?usp=drive_link) [分流2](https://drive.google.com/file/d/1zU_TVs8zIIAM1xKYzYwdKRVys4KDFQdv/view?usp=sharing)

[匯入虛擬機圖解](https://hackmd.io/@Flydragon/how2ovf)

本次課程需要以下工具，請在上課前自行安裝或直接使用我提供的虛擬機檔案

1. GNU
```
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install build-essential
```
2. Radare2
```
git clone https://github.com/radareorg/radare2
sudo ./radare2/sys/install.sh
```
3. GDB-peda
```
git clone https://github.com/scwuaptx/Pwngdb.git ; cp ~/Pwngdb/.gdbinit ~/
git clone https://github.com/scwuaptx/peda.git ~/peda ; echo "source~/peda/peda.py" >> ~/.gdbinit ; cp ~/peda/.inputrc ~/
```
4. Pwntools (with Python2)
```
sudo apt install python2
sudo apt install python-pip
python2 -m pip install --upgrade pip==20.3.4
python2 -m pip install --upgrade pwntools
```
5. IDA  

安裝有問題的話嘗試以下指令
```
sudo apt install xorg-dev
sudo apt install libxcb-xinerama0
```

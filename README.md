# MyFirstProgramSec

課程主要內容在簡報，此處主要是放指令和程式碼方便複製

## 環境
本次課程需要以下工具，請自行安裝或直接使用我提供的 ova

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

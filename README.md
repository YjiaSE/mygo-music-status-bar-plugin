该插件的作用是在linux的状态栏上显示歌词。

该插件配合此https://github.com/sogud/mygo-music-netease插件使用。
[![演示视频]()](src/demo.mp4)

使用步骤

### step1
安装mygo软件本体，接着安装https://github.com/sogud/mygo-music-netease此插件。
执行以下安装指令
```bash
sudo apt update
sudo apt install -y curl unzip gjs libglib2.0-bin \
  gnome-shell-extension-prefs gir1.2-soup-3.0 gir1.2-adw-1
```
### step2
安装顶栏扩展
```bash
gnome-extensions install \
  dist/mygo-panel-lyrics@local.shell-extension.zip
```
保存工作，**注销并重新登录 Ubuntu**，然后执行：
```bash
gnome-extensions enable mygo-panel-lyrics@local
gnome-extensions info mygo-panel-lyrics@local
```
状态应为 `ACTIVE`。打开设置：
```bash
gnome-extensions prefs mygo-panel-lyrics@local
```
### step3 
打开mygo的插件并授权。



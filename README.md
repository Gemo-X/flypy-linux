# 小鹤音形fcitx rime挂接版
小鹤音形挂接内容来自官方网盘。
http://flypy.ys168.com/

Linux小鹤音形需要挂载使用,Rime是个优秀的输入工具，在Mac/Windos/Linux/Andrido/ios平台都有对应的实现。  
Linux平台的Rime依赖fcitx。  

## 更新记录
https://flypy.com/bbs/forum.php?mod=viewthread&tid=8&extra=page%3D1

## Linux环境
- Archlinux
    - Manjaro

**安装依赖**
安装fcitx输入法框架和rime输入法
```sh
sudo pacman -S fcitx-rime
sudo pacman -S fcitx-configtool
```
**配置fcitx**
在程序里找到fctix配置，如果是英文系统，需要取消`only show current language`的勾选，中文系统则无需改变

将`rime-data`目录下的所有`yaml`和`txt`复制到`rime`的`rime-date`目录:
```sh
$ sudo cp *.yaml *.txt /usr/share/rime-data/
```

将`build`文件夹下所有的`bin`文件放到`rime`的`build`目录
```sh
 $ sudo cp /build/*.bin /usr/share/rime-data/build/
 ```

以上词库挂接后重启fcitx生效。

**美化设置**

fcitx用户目录
```
 ~/.config/fcitx/rime/             
 ```

rime的皮肤用的是fcitx的皮肤，自定义皮肤目录为:
```sh
/usr/share/fcitx/skin
```

**Rime配置**
禁用Rime的英文模式
rime的英文模会将`Shift`键触发为rime的英文模式。
从输入方案中 `engine/processor`列表里注视`ascii_composer`

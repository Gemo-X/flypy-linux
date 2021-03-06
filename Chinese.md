# 小鹤音形Linux挂接版镜像
[英文介绍](https://github.com/imaojun/flypy-linux/blob/master/README.md)

本仓库为小鹤双拼`GNU/Linux`挂接版镜像,挂接内容均来自官方网盘。 

- 网盘地址：
http://flypy.ys168.com/  

## 备注
更新到9.9g版本后，小鹤双拼已经移除Plus版本的配置信息和对应码表。


## 支持的输入法框架
`GNU/Linux`下小鹤音形没有开箱即用的程序，需要挂载Rime(中州韵)或者Yong(小小输入法使用。

目前已经在以下输入法框架下测试通过：

- [x] Fcitx-Rime
- [x] IBUS-Rime
- [x] YONG




## 小鹤双拼版本更新

官网更新说明:
https://flypy.com/bbs/forum.php?mod=viewthread&tid=8&extra=page%3D1


## 结构

小鹤双拼挂接RIME:
```
fcitx/rime-data
├── build
│   ├── flypydz.prism.bin
│   ├── flypydz.reverse.bin
│   ├── flypydz.table.bin
│   ├── flypy.prism.bin
│   ├── flypy.reverse.bin
│   └── flypy.table.bin
├── default.yaml
├── flypy.schema.yaml
├── flypy_sys.txt
├── flypy_top.txt
├── flypy_user.txt
└── rime.lua

```
小鹤双拼挂接Ibus:
```
ibus
├── bus
│   ├── 484233f2569a47908894dd244239e2fd-unix-0
│   └── 8ab79d3e156c46588cf333151756725f-unix-0
└── rime
    ├── build
    ├── default.custom.yaml
    ├── default.custom.yaml.example
    ├── flypy.schema.yaml
    ├── flypy_sys.txt
    ├── flypy_top.txt
    ├── flypy_user.txt
    ├── installation.yaml
    ├── luna_pinyin.userdb
    ├── rime-data
    ├── rime.lua
    ├── trash
    └── user.yaml
```

小鹤双拼挂接小小输入法:
```
yong
├── mb
│   ├── english.txt
│   ├── pinyin.txt
│   ├── pypre.bin
│   ├── xhbc.txt
│   ├── xhup.ini
│   ├── xhup.txt
│   ├── xhzcm.txt
│   └── yb.txt
├── skin
│   ├── ....
└── yong.ini

```



## 安装和使用

详情参看wiki:

https://github.com/imaojun/flypy-linux/wiki


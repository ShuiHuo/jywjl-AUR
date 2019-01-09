# jywjl-AUR

[局域网精灵](https://jywjl.github.io/) Linux 版的打包。

## 使用方式

仅限 archlinux 用户

1. 克隆仓库：
```shell
$ git clone https://github.com/ShuiHuo/jywjl-AUR.git
$ cd jywjl-AUR
```

2. 创建包：
```shell
$ makepkg
```

部分地区可能需要用代理创建包：
```shell
$ proxychains makepkg
```

3. 安装：
```shell
# pacman -U jywjl-1.0.0-2-x86_64.pkg.tar.xz
```

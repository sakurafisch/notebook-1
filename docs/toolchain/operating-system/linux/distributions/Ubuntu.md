# Ubuntu

- 务必使用LTS版本。（还是LTS最不折腾了。）
- 系统安装时推荐进行最小安装，并在安装时一并安装上第三方驱动。
- 发行版版本 `lsb_release -a` `uname -r` `do-release-upgrade`

```sh
sudo apt install vim  # 修正现代键盘兼容问题。
sudo apt install gnome-tweaks
sudo apt install kleopatra

sudo snap install --classic code
sudo snap install --classic code-insider
sudo snap install libreoffice
```

## apt

> The `apt` command is meant to be pleasant for end users and does not need
> to be backward compatible like `apt-get(8)`.

- 镜像 <https://mirror.tuna.tsinghua.edu.cn/help/ubuntu/>
- `apt update`, `apt upgrade`
- `apt search`
- `apt list --upgradable`, `apt list --installed`
- `apt install <package> --reinstall`
- `apt-mark auto <package>`
- `apt remove [--purge] "packagename-*"`

```conf
# /etc/apt/apt.conf
Acquire::http::Proxy "http://user:pass@host:port";
```

## snap

Perhaps snap is the future?

```sh
sudo snap set system proxy.http "http://host:port"
sudo snap set system proxy.https $HTTPS_PROXY
```

## 中文字体

- ttf-wps-fonts <https://github.com/IamDH4/ttf-wps-fonts>

## 中文输入法

保持使用Ibus为宜。
使用RIME输入法。

```sh
sudo apt install ibus-rime
ibus-setup
```

## 工具

```sh
apt install screenfetch
```

## 常用软件

``` txt
linux-generic (depends on linux-image-generic and linux-headers-generic)
linux-source

python python-pip
python3 python3-pip
```

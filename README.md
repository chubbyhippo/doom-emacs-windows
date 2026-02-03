# doom-emacs-windows
https://github.com/emacs-mirror/emacs/blob/master/nt/INSTALL.W64
```shell
mkdir emacs
```
```shell
cd emacs
```
```shell
git config --global core.autocrlf false
```
```shell
git clone --branch emacs-30.1 --depth 1 https://github.com/emacs-mirror/emacs.git .
```
```shell
./autogen.sh
```
```shell
sed -i 's/\r$//' configure.ac autogen.sh
```
```shell
./configure --prefix=/c/emacs \
            --with-native-compilation \
            --without-dbus

```
```shell
make -j$(nproc)
```
```shell
make install
```
```shell
git clone --depth 1 https://github.com/doomemacs/doomemacs ~/.config/emacs
~/.config/emacs/bin/doom install
```

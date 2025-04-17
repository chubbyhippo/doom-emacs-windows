# doom-emacs-windows
https://github.com/emacs-mirror/emacs/blob/master/nt/INSTALL.W64
```shell
mkdir /c/emacs
```
```shell
cd /c/emacs
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
./configure --prefix=/c/programs/emacs \
            --with-native-compilation \
            --without-dbus \
            CFLAGS="-O2 -static" \
            LDFLAGS="-static -static-libgcc -static-libstdc++" \
            --enable-static

```
```shell
make -j$(nproc)
```
```shell
make install
```

# doom-emacs-windows
https://github.com/emacs-mirror/emacs/blob/master/nt/INSTALL.W64
```shell

```
```shell
git clone --branch emacs-30.1 --depth 1 git://git.sv.gnu.org/emacs.git
```
```shell
./autogen.sh
```
```shell
./configure --prefix=/c/emacs \
            --with-native-compilation \
            --without-dbus
```

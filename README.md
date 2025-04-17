# doom-emacs-windows
https://github.com/emacs-mirror/emacs/blob/master/nt/INSTALL.W64
```shell
 pacman -S --needed base-devel \
  mingw-w64-x86_64-toolchain \
  mingw-w64-x86_64-xpm-nox \
  mingw-w64-x86_64-gmp \
  mingw-w64-x86_64-gnutls \
  mingw-w64-x86_64-libtiff \
  mingw-w64-x86_64-giflib \
  mingw-w64-x86_64-libpng \
  mingw-w64-x86_64-libjpeg-turbo \
  mingw-w64-x86_64-librsvg \
  mingw-w64-x86_64-libwebp \
  mingw-w64-x86_64-lcms2 \
  mingw-w64-x86_64-libxml2 \
  mingw-w64-x86_64-zlib \
  mingw-w64-x86_64-harfbuzz \
  mingw-w64-x86_64-libgccjit \
  mingw-w64-x86_64-sqlite3 \
  mingw-w64-x86_64-libtree-sitter
```
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

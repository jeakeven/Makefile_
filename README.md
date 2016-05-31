# Makefile_
makefile learning, include automake and autoconf

autoconf编译执行顺序为（需要修改configure.ac文件）：
autoscan; aclocal; autoconf; autoheader; automake --add-missing; ./configure; make; ./helloworld;


Autoconf和Automake安装（mac）

需要安装m4,autoconf, automake,libtool四个组件

1、安装m4
curl -O http://mirrors.kernel.org/gnu/m4/m4-1.4.13.tar.gz
tar -xzvf m4-1.4.13.tar.gz
cd m4-1.4.13
./configure --prefix=/usr/local
make
sudo make install

2、安装autoconf
curl -O http://mirrors.kernel.org/gnu/autoconf/autoconf-2.65.tar.gz
tar -xzvf autoconf-2.65.tar.gz
cd autoconf-2.65
./configure --prefix=/usr/local # ironic, isn't it?
make
sudo make install

3、安装automake，可能需要重启terminal
# here you might want to restart your terminal session, to ensure the new autoconf is picked up and used in the rest of the script
curl -O http://mirrors.kernel.org/gnu/automake/automake-1.11.tar.gz
tar xzvf automake-1.11.tar.gz
cd automake-1.11
./configure --prefix=/usr/local
make
sudo make install

4、安装lib tool
curl -O http://mirrors.kernel.org/gnu/libtool/libtool-2.2.6b.tar.gz
tar xzvf libtool-2.2.6b.tar.gz
cd libtool-2.2.6b
./configure --prefix=/usr/local
make
sudo make install

至此安装成功

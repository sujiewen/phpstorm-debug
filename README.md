# phpstorm-debug


PhpStorm 2022.3.3
macOS 11.6
PHP 7.3.3
xdebug 3.1.6
本地server地址：localhost:9011


vim /usr/local/etc/php/7.3/php.ini

[xdebug]
<br>
;zend_extension = /usr/local/lib/php/pecl/20180731/xdebug.so
enable = On
xdebug.remote_handler = "dbgp"
xdebug.client_host = "localhost"
xdebug.client_port = 9001
xdebug.idekey = PHPSTROM
xdebug.start_with_request=yes
xdebug.mode=debug


xdebug 安装

php -i 
把显示内容拷贝到 https://xdebug.org/wizard， 点击Anaylse my phpinfo() output


1，Download xdebug-3.1.6.tgz (https://xdebug.org/files/xdebug-3.1.6.tgz)
  
  
2，Install the pre-requisites for compiling PHP extensions.
  On your Mac, we only support installations with 'homebrew', and brew install php && brew install autoconf should pull in the right packages.
3，Unpack the downloaded file with tar -xvzf xdebug-3.1.6.tgz
4，Run: cd xdebug-3.1.6
5，Run: phpize (See the FAQ if you don't have phpize).
6，Run: ./configure
7，Run: make
8，Run: cp modules/xdebug.so /usr/local/lib/php/pecl/20180731
9，Update /usr/local/etc/php/7.3/php.ini to have the line:
zend_extension = xdebug

具体参考  https://xdebug.org/wizard







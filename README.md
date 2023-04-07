# phpstorm-debug


<br>
PhpStorm 2022.3.3
<br>
macOS 11.6
<br>
PHP 7.3.3
<br>
xdebug 3.1.6
<br>
本地server地址：localhost:9011


<br>
vim /usr/local/etc/php/7.3/php.ini

[xdebug]
<br>
;zend_extension = /usr/local/lib/php/pecl/20180731/xdebug.so
<br>
enable = On
<br>
xdebug.remote_handler = "dbgp"
<br>
xdebug.client_host = "localhost"
<br>
xdebug.client_port = 9001
<br>
xdebug.idekey = PHPSTROM
<br>
xdebug.start_with_request=yes
<br>
xdebug.mode=debug




<br>
<br>
<br>
xdebug 安装

php -i 
把显示内容拷贝到 https://xdebug.org/wizard， 点击Anaylse my phpinfo() output


<br>
1，Download xdebug-3.1.6.tgz (https://xdebug.org/files/xdebug-3.1.6.tgz)
<br>
2，Install the pre-requisites for compiling PHP extensions.
<br>
  On your Mac, we only support installations with 'homebrew', and brew install php && brew install autoconf should pull in the right packages.
  <br>
3，Unpack the downloaded file with tar -xvzf xdebug-3.1.6.tgz
<br>
4，Run: cd xdebug-3.1.6
<br>
5，Run: phpize (See the FAQ if you don't have phpize).
<br>
6，Run: ./configure
<br>
7，Run: make
<br>
8，Run: cp modules/xdebug.so /usr/local/lib/php/pecl/20180731
<br>
9，Update /usr/local/etc/php/7.3/php.ini to have the line:
<br>
zend_extension = xdebug
<br>
具体参考  https://xdebug.org/wizard







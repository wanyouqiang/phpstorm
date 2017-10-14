# 使用PHPStorm+xdebug+PHP进行代码调试
### 开启xdebug扩展

在MAMP的php.ini配置文件中:
	`
	zend_extension="/Applications/MAMP/bin/php/php7.1.8/lib/php/extensions/no-debug-non-zts-20160303/xdebug.so"
	xdebug.remote_enable = On
	xdebug.remote_handler = dbgp
	xdebug.remote_host= localhost
	xdebug.remote_port = 9001
	xdebug.idekey = PHPSTORM
	xdebug.profiler_enable = On
	xdebug.profiler_enable_trigger = On
	`

### 配置PhpStorm
* PhpStorm的Xdebug端口必须要和配置文件中的端口保持一致
* Servers配置端口要和本地apache服务器上一致（也可以进行远程调试）
* Debug选项中的DBGp proxy 中IDE key:phpStorm,Host:localhost,port与Servers一致

### 配置服务器  

在Run configuration里新增web application server

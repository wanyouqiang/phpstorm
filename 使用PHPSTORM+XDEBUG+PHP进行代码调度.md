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

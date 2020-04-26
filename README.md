MySQL-Research
==============

MySQL数据库源代码学习研究(包括代码注释、文档、用于代码分析的测试用例)
#MySQL代码结构
•build: 内含有各个平台、各种编译器下进行编译的脚本。如compile-pentium-debug表示在pentium架构上进行调试编译的脚本。
•client: 客户端工具，如mysql,mysqladmin之类。
•cmd-line-utils: readline,libedit工具。
•config: 给aclocal使用的配置文件。
•dbug: 提供一些调试用的宏定义。
•Docs: MySQL在不同平台下的参考手册
•extra: 提供innochecksum,resolveip等额外的小工具。
•include: 包含的头文件
•libmysql: 库文件，生产libmysqlclient.so。
•libmysql_r: 线程安全的库文件，生成libmysqlclient_r.so。
•libmysqld: 嵌入式MySQL Server库.
•libservices: 5.5.0中新加的目录，实现了打印功能。
•man: 适合man命令查看的帮助文件。
•mysql-test: mysqld的测试工具套件。
•mysys: 为实现跨平台，MySQL自己实现了一套常用的数据结构和算法，如string, hash等。还包含一些底层函数的跨平台封装,一般以my_开头。
•netware: 在netware平台上进行编译时需要的工具和库。
•plugin: MySQL 5.1开始支持一个插件式API接口,不需要重启mysqld即可动态载入插件,FullText就是一个例子。
•pstack: GNU异步栈追踪工具。
•regex: 正则表达式实现(来自多伦多大学Henry Spencer大牛的源码)。
•scripts: 提供脚本工具，如mysql_install_db/mysqld_safe等。
•server-tools: 包含instance_manager子目录,负责实例的本地和远程管理。
•sql: MySQL Server主要代码，将会生成mysqld文件。
•sql-bench: 一些基准测试代码代码,主要是Perl程序(虽然后缀是sh)。
•sql-common: 存放部分服务器端和客户端都会用到的代码,有些地方的同名文件是这里lin过去的。
•storage: 存储引擎所在目录。
•strings: string库,包含很多字符串处理的函数。
•support-files: my.cnf示例配置文件及编译所需的一些工具。
•tests: 测试文件所在目录。
•unittest: 单元测试文件。
•vio: 虚拟io系统，是对network io的封装,把不同的协议封装成统一的IO函数。
•win: 在windows平台编译所需的文件和一些说明。
•zlib: zlib算法库(GNU)

# InnoDB目录结构
    •btr: B+树的实现
    •buf: 缓冲池的实现,包括LRU算法,Flush刷新算法等
    •dict: InnoDB内存数据字典的实现
    •dyn: InnoDB动态数组的实现
    •fil: InnoDB文件数据结构以及对于文件的一些操作
    •fsp: 对InnoDB物理文件的管理,如页/区/段等(即File Space)
    •ha: 哈希算法的实现
    •handler: 继承与MySQL的handler,实现handler API与Server交互
    •ibuf: 插入缓冲(Insert Buffer)的实现
    •include: InnoDB所有头文件都放在这个目录,是查找结构定义的最佳地点
    •lock: InnoDB的锁实现及三种锁算法实现
    •log: 日志缓冲(Log Buffer)和重做日志组(Redo Log)的实现
    •mem: 辅助缓冲池(Additional Memory Pool)的实现,用来申请一些内部数据结构的内存
    •mtr: 事务的底层实现(日志,缓冲)
    •os: 封装一些对于操作系统的操作
    •page: 页的实现,研究InnoDB文件结构,这个目录至关重要
    •pars: 重载部分MySQL的SQL Parser(有待商榷)
    •que: Query graph,基本上没啥用
    •read: 读取游标的实现
    •rem: 行管理操作(比较操作,打印等)
    •row: 对于各种类型行数据操作的实现
    •srv: InnoDB后台线程,启动服务,Master Thread,SQL队列等
    •sync: InnoDB互斥变量(Mutex)的实现,基本同步机制
    •thr: InnoDB封装的可移植线程库
    •trx: 事务的实现
    •usr: Session管理
    •ut: 各种通用小工具

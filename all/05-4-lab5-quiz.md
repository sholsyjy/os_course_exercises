#lab５ 用户进程　在线练习
## 选择题

---

下列叙述中正确的是()  s2

- [ ] lab５建立了用户进程，且0~3GB都是用户可访问空间，用户进程可进行正常读写
- [ ] lab５建立了用户进程，且3GB～４GB都是内核可访问空间，内核可进行正常读写
- [x] lab5中的第一个用户进程是内核创建的。
- [x] lab5中的用户进程可通过fork创建新的用户进程。

> 3,4


lab5通过do_execve函数执行新的程序，为此需要完成（） s3

- [x] 更新用户进程的context
- [x] 更新用户进程的代码内容
- [x] 更新用户进程的数据内容
- [ ] 更新用户进程的页表基址

> 1,2,3,4

lab5通过do_icode函数执行新的程序，为此需要完成（）s4

- [x] 设置用户堆栈
- [x] 修改页表
- [x] 根据ELF执行文件的格式描述分配内存并填写内容
- [x] 设置用户态的EFLAG寄存器不可屏蔽中断

> 都包括


关于进程管理的COW(Copy On Write)机制叙述正确的是（）s6

- [ ] 父进程创建子进程需要复制父进程的内存空间
- [ ] 父进程创建子进程需要给子进程分配内核堆栈
- [ ] 父进程创建子进程需要给子进程分配用户堆栈
- [x] 父进程创建子进程需要创建子进程的页表,但不复制父进程内存空间

> 4



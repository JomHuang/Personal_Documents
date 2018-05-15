# windbg 常用方法和案例
1. 案例
- http://www.cnblogs.com/ants/p/4961487.html windbg实际应用

2. 常用命令
- !analyze –v  自动分析 kv  查看堆栈
- !runaway  显示所有线程的CPU消耗
- !handle e00 f 显示句柄详细详细
- !cs 00bcd034 临界对象
- !teb查看TEB的结构
- bp 下断点，还有条件断点
- !address 显示整个地址空间和使用摘要的信息
- dd 按字节查看
- dt 查看结构       

3. 基本使用方法
- 打开windbg，attach到指定进程，设置捕获异常并输出的命令：sxe -c "!pe;!clrstack;g" clr
也可以直接使用.logopen命令将系统代码中的内部异常日志输出到文件中。





# ch05 Demo

```bash
make all
size demo01_memory_zone
./demo01_memory_zone

gdb ./demo02_stack_frame
# (gdb) break recurse
# (gdb) run
# (gdb) bt
# (gdb) x/32xb $sp

valgrind --leak-check=full ./demo04_heap_leak
./demo05_static
```

## demo03 栈溢出（慎用）

在函数内定义超大局部数组或无限递归会 SIGSEGV；仅用于 gdb 观察 `bt`/`info registers sp lr`。

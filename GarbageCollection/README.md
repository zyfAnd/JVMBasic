1. 哪些内存需要被回收？
2. 什么时候被回收？
3. 如何回收？


什么是垃圾呢？
 1. 程序运行中没有任何指针指向的对象 An object is considered garbage when it can not be reached from any pointer in the running program.
为什么需要GC？
 1. 因为程序运行的空间是有限的，如果不进行垃圾回收 内存空间迟早要被消耗完了 那么正常的应用程序就不能进行运行了 （Stack Over Flow）
1. 哪些内存需要被回收？
2. 什么时候被回收？
3. 如何回收？


什么是垃圾呢？
 1. 程序运行中没有任何指针指向的对象 An object is considered garbage when it can not be reached from any pointer in the running program.
为什么需要GC？
 1. 因为程序运行的空间是有限的，如果不进行垃圾回收 内存空间迟早要被消耗完了 那么正常的应用程序就不能进行运行了 （Stack Over Flow）/ Out of Memory 

Java 是怎么样实现自动的内存管理的呢？
1. 垃圾回收器会自动回收不在使用的对象

垃圾回收器关心哪些内存区域
1. 堆空间
2. 元空间（方法区）、


垃圾回收的算法
1. 这么判断对象是否可以被回收呢（哪些对象是垃圾呢？）-->  标记阶段 标记出出来垃圾 --> 引用计数法/可达性分析算法
2. 这么回收呢 -->清除阶段

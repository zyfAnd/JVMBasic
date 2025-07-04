1. 判断对象的类是否加载 未加载的 -> loading --> linking(verification/preparation/resolution) -> initiation 
2. 为对象分配内存空间 堆内存 如何内存是规整的 就是用指针碰撞 Serial， Pra，  如何不是规整的 就要使用 空闲列表的方式 比如CMS 垃圾收集器
3. 处理并发安全问题
4. 初始化分配空间 给属性默认初始化数值
5. 设置对象的对象头 对象头所属的类 
6. 执行init 方法进行初始化
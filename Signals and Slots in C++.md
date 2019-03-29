##Signals and Slots in C++


在查看Qt方面的资料时，阅读了https://www.cnblogs.com/tr0217/p/9223937.html 这片文章，其中对作者的一些观点感兴趣，摘录一段，“那么Qt以如此之高代价实现的信号和槽机制到底是什么高档玩意呢？说白了就是一种发布/订阅机制而已，对于没有从语言层面上支持调用栈上的发布/订阅机制的编程语言来说，一般通过两种方式来实现——Listener模式和回调函数。java swing就是典型的Listener模式，这个很显然；如果说MFC的Message Map是回调函数，可能会遇到争议。Message Map提供了消息码到消息处理函数指针的映射，消息循环从Message Map中查找到处理某个消息的所有函数指针，然后依次调用。消息循环是框架提供的，只是通过Message Map的形式传进去一个函数指针而已，虽然没有直接调用SetXXXCallBack，不影响它仍然是回调函数。”，所以对信号与槽进行一些了解。

主要参照库为http://sigslot.sourceforge.net/。





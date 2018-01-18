# JavaList面试题汇总
### 1、你知道的List都有哪些？
ArrayList、LinkedList、Vector等。 

### 2、List和Vector有什么区别？
Vector是List接口下线程安全的集合。

### 3、List是有序的吗？
List是有序的。 

### 4、ArrayList和LinkedList的区别？分别用在什么场景？
ArrayList和LinkedList数据结构不一样，前者用在查询较多的场合，后者适用于插入较多的场合。 

### 5、ArrayList和LinkedList的底层数据结构是什么？
ArrayList使用的是数组结构，LinkedList使用的是链表结构。

### 6、ArrayList默认大小是多少，是如何扩容的？
Jdk1.7之前ArrayList默认大小是10，JDK1.7之后是0，JDK差异，每次约按1.5倍扩容。

### 7、List是线程安全的吗？如果要线程安全要怎么做？
List中的Vector才是线程安全的，其他要实现线程安全使用工具类Collections.synchronizedList(new ArrayList())方法。

### 8、怎么给List排序？
使用List自身的sort方法，或者使用Collections.sort(list)方法; 

### 9、Arrays.asList方法后的List可以扩容吗？
Arrays.asList使用的是final数组，并且不支持add方法，不支持扩容。

### 10、List和Array之间如何互相转换？
List>Array使用toArray方法，Array>List使用Arrays.asList(array)方法，由于它是固定的，不固定的可以使用new ArrayList(Arrays.asList(array))。

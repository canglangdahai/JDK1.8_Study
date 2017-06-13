　　JDK源码阅读-`ArrayList`
===

##简介
ArrayList底层是Object数组维护,数组内存空间地址是连续的，数组可以按索引直接查找，故查找快。又增删时会涉及数组增容以及拷贝元素，因此增删慢。下面看源码：
##命名
```Java
public class ArrayList<E> extends AbstractList<E>
implements List<E>, RandomAccess, Cloneable, java.io.Serializable {
```


#### 介绍Js数据类型

共有8大类型：Undefined、null、Boolean、Number、string、object、symbol、bigInt

- symbol 代表的是创建后独一无二且不可变的数据类型，解决全局变量冲突
- bigInt 数字类型，可以表示任意精度格式的证书
- 栈 原始类型（undefined、null、boolean、number、string）
  - 原始数据类型直接存储在栈中，占据空间大小，属于频繁使用的数据
- 堆 引用数据类型（对象、数组、函数）
  - 引用类型存储在堆中，占据空间大小不确定。如果放在栈中，影响性能。引用类型在栈中存储了指针，指向堆中该实体的起始地址，取得地址后从堆中获得实体


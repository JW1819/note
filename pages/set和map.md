#### Set

特点：类似于数组，但是成员唯一不重复

生成方式：

- let s = new Set()
- let items = new Set( [1, 2, 3, 4, 5, 5, 4] )

属性：

- Set.protptype.constructor  构造函数，默认为Set函数
- Set.protptype.size  返回成员总数

方法：

- add(value)
- delete(value)
- has(value)
- clear()

与数组的联动

Array.from()可以将Set结构转换为数组

由此提供数组去重方法： Array.from(new Set(array))



#### Map

特点：类似于对象。对象中键值对的键名只能是字符串，而Map中不限于字符串。

注意：只有对同一个对象的引用，Map结构才将其视为同一个键。

例如： map.set(['a'], 5555);       map.get(['a'])  // undefined

方法：

- size属性
- set(key, value)
- has(key)
- get(key)
- delete(key)
- clear()

遍历：

- keys()
- value()
- entries()
- foreach()


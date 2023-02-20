#### Promise对象

定义：promise对象是一个构造函数，用于生成promise实例。

基本用法：

```javascript
var promise = new Promise(function(resolve, reject) {
​	if (success) {
		resolve(value)
	} else {
    reject(erroe)
  }
});
promise.then(function(value) {
  success
}, function(value) {
  failure
})
```

promise接受一个函数作为参数，该函数的两个参数分别为resolve方法和reject方法，异步成功则用resolve方法（pending => resolved），异步失败则用reject方法(pending => rejected)。

promise实力生成之后，可以用then方法分别制定resolve方法和reject方法的回调函数。then方法返回的是promise对象，因此可是继续掉用then方法，实现链式掉用。

catch方法：捕捉错误。是then的别名，用于指定发生错误的回调函数

promise.then().catch()



#### Async

用于取代回调函数的另一种方法。函数名前面加上async，表明函数内部有异步操作异步操作返回一个promise对象，前面用await关键字注明。一旦遇到await就会先返回，等待触发的异步操作完成，再接着执行后面的语句。相当于异步的同步化操作。
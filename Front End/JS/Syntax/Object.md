# js对象

```js
ctor == constructor
dtor ==  destructor
```

hasOwnProperty：是用来判断一个对象是否有你给出名称的属性或对象。不过需要注意的是，此方法无法检查该对象的原型链中是否具有该属性，该属性必须是对象本身的一个成员。

isPrototypeOf:是用来判断要检查其原型链的对象是否存在于指定对象实例中，是则返回true，否则返回false。
# 数组array

### 数组初始化
```
var arrayObj = new Array();　//创建一个数组

var arrayObj = new Array([size]);　//创建一个数组并指定长度，注意不是上限，是长度

var arrayObj = new Array([element0[, element1[, ...[, elementN]]]]);　创建一个数组并赋值

要说明的是，虽然第二种方法创建数组指定了长度，但实际上所有情况下数组都是变长的，也就是说即使指定了长度为5，仍然可以将元素存储在规定长度以外的，注意：这时长度会随之改变。
```

### 数组元素访问
```
var testGetArrValue=arrayObj[1]; //获取数组的元素值

arrayObj[1]= "这是新值"; //给数组元素赋予新的值
```

### 添加数组元素
```
arrayObj.push([item1 [item2 [. . . [itemN ]]]]);// 将一个或多个新元素添加到数组结尾，并返回数组新长度

arrayObj.unshift([item1 [item2 [. . . [itemN ]]]]);// 将一个或多个新元素添加到数组开始，数组中的元素自动后移，返回数组新长度

arrayObj.splice(insertPos,0,[item1[, item2[, . . . [,itemN]]]]);//将一个或多个新元素插入到数组的指定位置，插入位置的元素自动后移，返回""。
```

### 删除数组元素
```
arrayObj.pop(); //移除最后一个元素并返回该元素值

arrayObj.shift(); //移除最前一个元素并返回该元素值，数组中元素自动前移

arrayObj.splice(deletePos,deleteCount); //删除从指定位置deletePos开始的指定数量deleteCount的元素，数组形式返回所移除的元素
```

### 数组的截取和合并
```
arrayObj.slice(start, [end]); //以数组的形式返回数组的一部分，注意不包括 end 对应的元素，如果省略 end 将复制 start 之后的所有元素

arrayObj.concat([item1[, item2[, . . . [,itemN]]]]); //将多个数组（也可以是字符串，或者是数组和字符串的混合）连接为一个数组，返回连接好的新的数组
```

### 数组的拷贝
```
arrayObj.slice(0); //返回数组的拷贝数组，注意是一个新的数组，不是指向

arrayObj.concat(); //返回数组的拷贝数组，注意是一个新的数组，不是指向
```

### 数组元素的排序
```
arrayObj.reverse(); //反转元素（最前的排到最后、最后的排到最前），返回数组地址

arrayObj.sort(); //对数组元素排序，返回数组地址
```

### 数组元素的字符串化
```
arrayObj.join(separator); //返回字符串，这个字符串将数组的每一个元素值连接在一起，中间用 separator 隔开。

toLocaleString 、toString 、valueOf：可以看作是join的特殊用法，不常用
```

### 遍历数组,json

```js
$.each(arr, function(i, item){
});

专用于jQuery对象的遍历
arr.each(function(i,obj){})

arr.each(function(key,values){})
```
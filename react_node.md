# React框架中涉及JS的知识点

react中推荐使用关键字 const,其次let,最好不用var

let有块作用域，var无块作用域

const具有块级作用域，但只能赋值一次

1. 用于常量，如PI
2. 对于一些对象、函数用const申明，避免被修改，对象值可新增，但已有属性不能被赋值

---



展开,三个点语法，展开数据、展开对象

function sum(...arr)

---

解构赋值

```javascript
let [a,b]=[b,a];

let obj = {
  name:'孙金榜',
  age: '29'
}

const {name,age}=obj;
```

---

箭头函数，弥补普通函数的缺点，能用箭头函数就用箭头函数

```javascript
(参数) => 返回值（有返回值的表达式)
```

特点：

1. 没有arguments(类数组对象，数组的方法没有)参数，普通有
2. this永远指向window对象，箭头函数的this等于外层函数的this
3. 箭头中的this无法通过call()、apply()、bind修改
4. 无法作为构造函数

---

模块化

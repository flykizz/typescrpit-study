# 解释型问题

# 1.下面代码会不会报错？怎么解决？

```
const obj = {
    a: 1,
    b: 'string',
};

obj.c = null;
```

# 2.下面代码中，foo 的类型应该如何声明?

```
function foo (a: number) {
    return a + 1;
}

foo.bar = 123;
```

# 3.下面代码中，foo 的类型如何声明

```
let foo = {};

for (let i = 0; i< 100; i++) {
    foo[String(i)] = i;
}
```

# 4.下面代码中，foo 的类型如何声明

```
function fn(value: number): string {
    return String(value);
}
const foo = fn;
```

# 5.下面代码会导致 TS 编译失败，如何修改 getValue 的类型声明。

```
function getValue() {
    return this.value;
}

getValue();
```

# 6.如何声明 foo 的类型？

```
const foo = new Map();
foo.set('bar', 1);
```

# 7.如何声明 getProperty，以便能检查出第八行将会出现的运行错误。

```
function getProperty(obj, key) {
    return obj[key].toString();
}

let x = { a: 1, b: 2, c: 3, d: 4 };

getProperty(x, "a");
getProperty(x, "m");
```

```

```

# 8.下面代码里「date is Date」有什么作用？

```
function isDate(date: any): date is Date {
  if (!date) return false;
  return Object.prototype.toString.call(date) === '[object Date]';
}
```

# 9.如何处理才能在 TS 中引用 CSS 或者 图片使之不报错？

```
import "./index.scss";
import imgPath from "./home.png";
```

```

```

# 10.编写 d.ts 来声明下面的 js 文件

```
class Foo {
}
module.exports = Foo;
module.exports.Bar = 1;
```

```

```

# 11.如何实现 module alias?编译成 JS 能否直接运行？

```
import Bar from '@src/Bar';
```

#### 




# JS 对象基本用法

## 声明对象的两种语法

```js
let obj = { name: "xiaoming", age: 18 };
let obj1 = new Object({
  name: "xiaoming",
});
```

## 如何删除对象的属性

```js
delete obj["name"];
delete obj.xxx;
```

## 如何查看对象的属性

- 查看自身所有属性

```js
Object.keys(obj);
```

- 查看自身+共有属性

```js
console.dir(obj);
```

- 查看属性

```js
obj["key"]; /*中括号语法*/

obj.key; /*点语法*/
```

## 如何修改或增加对象的属性

```js
/*直接赋值*/
obj["name"] = "xiaoming";
/*批量赋值*/
Object.assign(obj, { age: 18, gender: "man" });

/*修改隐藏属性*/
let common = { name: "xx", age: 18 };
let obj1 = Object.create(common);
obj.name = "jack";
```

## 'name' in obj 和 obj.hasOwnProperty('name') 的区别

- 'name' in obj 表示 name 属性是否存在于 obj 对象自身属性里面，不包括原型属性。

- obj.hasOwnProperty('name') 表示 name 是否为 obj 自身的属性，如果是自身属性返回 ture，是原型属性或不存在该属性，则返回 false。

```

```

# readmi-clouser
# JavaScript Recursion & Closure

# Recursion

Recursion вақте мешавад, ки function худашро call мекунад.

## Example

```js
function solution(num) {
  if (num == 0) {
    return 0;
  }

  return num + solution(num - 1);
}

console.log(solution(5));
```

---

# Чихе кор мекна?

Function суммаи рақамҳоро ҷамъ мекуна

```js
5 + 4 + 3 + 2 + 1
```

---

# num - 1 чияй

```js
solution(num - 1)
```

Ҳар бор num 1-то кам мешавад

```js
5
4
3
2
1
0
```

Вақте 0 шуд function stop мешавад

---

# Чихе ҷамъ (+) шдестай

Аввал:

```js
5 + 4 + 3 + 2 + 1
```

Баъд JavaScript ҳамара ҷамъ мекунад

```js
15
```

---

# Output

```js
15
```

---

# Closure

Closure вақте мешавад, ки function variable-и берунара истифода мебара

## Example

```js
function counter() {
  let count = 0;

  return function () {
    count++;
    console.log(count);
  };
}

const plus = counter();

plus();
plus();
plus();
```

---

# count++ чияй

```js
count++;
```

Яъне:

```js
count = count + 1
```

Ҳар бор 1-тф зиёд мешавад

---

# Output

```js
1
2
3
```

---



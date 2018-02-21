# Help me!

I was working on math task and was not able to solve it :(
Please, help me to implement "simple" counter.

```js
function count(s, pairs) {
  return 0; // number
}
```

*As first argument* you will take bit mask in string `s` (can contains only `1` or `0`).
*As second argument* you will take array of pairs (array, which contain many arrays with length equal 2). Each `pairs[q][0] !== pairs[w][0]` and each `pairs[h][0]` is prime.

Let's define number `N`
```js
  N = (pairs[0][0] ** pairs[0][1]) *
    (pairs[1][0] ** pairs[1][1]) *
    (pairs[2][0] ** pairs[2][1]) * /*
    ..... */ *
    (pairs[pairs.length - 1][0] ** pairs[pairs.length - 1][1])
```

Your task is to calculate - *how many* such integer numbers `k` exist (`0 <= k <= N`), which follow next condition: greatest common divisor of (`k + j` and `N`) is 1 if `s[j] === 1` *AND* greatest common divisor of (`k + j` and `N`) is *NOT* 1 if `s[j] === 0`.

Please, return *NOT* the actual number, but the number which is answer mod 1000000007.
```js
  // ... your solution
  // answer - task solution
  const result = answer % 1000000007;
  return result;
```

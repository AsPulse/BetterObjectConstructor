# BetterObjectConstructor

![npm](https://img.shields.io/npm/dw/better-object-constructor?color=%23c9003d&style=flat-square&label=Downloads)
![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/aspulse/BetterObjectConstructor?color=%23c9003d&label=Pull%20Requests&style=flat-square)
![npm (tag)](https://img.shields.io/npm/v/better-object-constructor?style=flat-square)
![npm bundle size](https://img.shields.io/bundlephobia/min/better-object-constructor?style=flat-square)
![GitHub](https://img.shields.io/github/license/aspulse/BetterObjectConstructor?style=flat-square)  

<br>

## How to use?
```ts
import type { BetterObjectConstructor } from 'better-object-constructor';

declare const Object: BetterObjectConstructor;
```

<br>

## What will change?
For example: 
```ts
const hoge: { a: string } = {
  a: 'fugafuga'
};

const hoge2 = Object.fromEntries(Object.entries(hoge));
```
Placed in this code, hoge and hoge2 should truly have the same type.    
But let's look at it in the editor. (Below is a sample in VSCode…)

---

Oh! We lost the type!  
But don't worry, if you add the code shown in the "How to use?" section...?

---

Welcome back, my lovely type definition.  
...That's the kind of package.


<br>

## Author
[Follow @\_AsPulse\_](https://twitter.com/_AsPulse_?ref_src=twsrc%5Etfw)

<br>

## License
BetterObjectConstructor is licensed under MIT.   
Please see [LICENSE](./LICENSE) for more info.
